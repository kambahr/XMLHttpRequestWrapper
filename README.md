# quenubesHTTP - XMLHttpRequest Wrapper

## A native javascript XMLHttpRequest wrapper to simplify making HTTP calls. 

Pass url, method, array of headers, and the data JSON to make an asynchronous HTTP call.

The following is a simple example.

    function postUserId(useId){
      let q = new quenubesHTTP ('api/makpostuserId','POST',['X-UserID:'+useId+''],{},
        function (res) {   
            if(res.statusCode == 200){
              /* Code for success */
            }else{
              /* Code for failure */
            }
        }        
      );
      q.call();
    }        

See usage.html for a more detailed example.
