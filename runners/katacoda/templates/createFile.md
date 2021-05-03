<%= text; %>

If the parent directories aren't already in the project, 'mkdir -p' will create them for you. 

`mkdir -p <%= filePath; %>`{{execute T1}}

You can either create a new file by right clicking on the folder <%= filePath; %> >> New >> File and name it '<%= fileName; %>'
or run this command in your terminal.

`touch <%= fileDir; %> `{{execute T1}}

You can open the newly created file, here: 
`<%= fileDir; %>`{{open}}

<% if(content){ %>

Switch to the IDE and click 'Copy to Editor'. It will insert the following text into the file <%= fileName; %>.

<pre class="file" data-filename="<%= fileDir; %>">
<%= content; %>
</pre>

It might not display the changed file immediately. Close the file and click on 'refresh tree' to refresh the files. 

<% } %>

<%= textAfter; %>