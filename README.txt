# This code is free software: you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation, either version 3 of the License, or
# (at your option) any later version.
# get-rfc is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
# You should have received a copy of the GNU General Public License
# along with this code.  If not, see <http://www.gnu.org/licenses/>.


This program can be used to fetch any rfc from the archives of the IETF

Usage:
  get-rfc [number] [format]
  
Options:
  number: any number, or a range of numbers enclosed in brackets (i.e., 123, [1-99], etc)
  format(optional): defaults to txt, options are: txt,html,pdf,ps

NOTE:
  Fetching the index can be done by passing 'index' as the number parameter, the format will be disregarded
