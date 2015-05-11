for l in $(echo $i); do echo '\\begin{code} \lstinputlisting{'${l}'}' >> codes.list; echo "\caption{$(echo $l | cut -d/ -f4- | tr _ ' ')}" >> codes.list; echo '\\end{code}' >> codes.list; done
