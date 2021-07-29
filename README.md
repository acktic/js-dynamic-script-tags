# js-dynamic-script-tags
Load javascript files dynamically  

`  

      let directory = "root/js/";
      let extension = ".js";
      let files = [
        'Example'
      ]

      for (var file of files) {
        let path = directory + file + extension;
        let script = document.createElement("script");
        script.type = "text/javascript";
        script.src = path;
        document.getElementsByTagName("head")[0].appendChild(script);
`
