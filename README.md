# formbuilder
Generate Form Creation Drag and Drop With Javascript <a href="http://hangsbreaker.github.io/formbuilder/">Demo</a>

# How to use
<pre>buildform([FORM ID], [JSON DATA], [LANG]);</pre>
# Example
<pre>&lt;form id="formbuilder" method="post" action=""&gt;&lt;/form&gt;
<script>
const form = {
                "title" : "Judul Formulir",
                "description" : "Deskripsi Formulir",
                "form" : [
                            {
                              "type" : "text",
                              "question" : "Nama",
                              "description" : "Isi dengan nama lengkap",
                              "required" : true,
                              "data":[]
                            },
                            {
                              "type" : "select",
                              "question" : "Kelamin",
                              "description" : "",
                              "required" : true,
                              "data" : [
                                          "Laki - laki",
                                          "Perempuan"
                                      ]
                            }
                          ]
              };

buildform("formbuilder", form, "id");
</script></pre>
# Add form
<pre>let formjson = {
                  "type" : "text",
                  "question" : "Telepon",
                  "description" : "Isi dengan nomor telepon",
                  "required" : false,
                  "data":[]
                },
  
formbuilder_add("formbuilder", formjson, "id");</pre>
