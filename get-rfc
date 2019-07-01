#!/bin/bash
if [ -z $1 ]
    echo "No arguements: Expected at least 1"
    echo "get-rfc [number] (format)"
    echo "Number can be a range, i.e. get-rfc [1-100] pdf"
    echo "Format options are: txt,html,ps,pdf"
    echo "    Format defaults to txt"
fi

case $1 in
    index)
        curl https://www.rfc-editor.org/in-notes/rfc-index.txt;;
esac

if [ -z $2 ]
then
    curl https://www.rfc-editor.org/rfc/rfc$1.text;;
else
    case $2 in
        pdf)
            curl https://www.rfc-editor.org/rfc/rfc$1.text.pdf;;
        txt|ps|html)
	    curl https://www.rfc-editor.org/rfc/rfc$1.$2;;
        *)
            echo "Format/extension not supported"
	    exit 1;;
    esac    
fi

ret=$?
if [ -nz $ret ]
    echo "Curl failed with code: $ret"
    echo "Check if rfc # is valid"
    exit $ret
fi
exit 0
