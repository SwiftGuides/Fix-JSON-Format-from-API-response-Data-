# Fix-JSON-Format-from-API-response-Data-
This will fix improper form of json format in response data and convert it to proper json form


```

        let dataTask = session.dataTask(with: request as URLRequest, completionHandler: { (data, response, error) -> Void in
            if (error != nil) {
                print(error)
            } else {
                
                //This below code will fix improper fromat of json 
                let json = String(data: data!, encoding: .utf8)
                print(json!)
                
                
            }
        })
        
        dataTask.resume()
        
        ```
