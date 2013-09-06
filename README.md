JSONP
=====

This is a tiny (0.8kB minified) standalone script allowing you to make JSONp calls without requiring a third party library.

Usage
-----

Include the json.js (or json.min.js) file or copy the code directly into your application.

    // Example
    JSONP.get('http://www.example.com',
              {
              'parameter_one': document.getElementById('parameter_one').value,
              'parameter_two': parameter_two,
              'parameter_three': 'testing'
              },
              function(response)
              {
                  if (response.error)
                  {
                        // Error!
                        alert(response.error);
                        return false;
                  }
                  else
                  {
                        // Success!
                        alert('Great success!');
                        return true;
                  }
              });
