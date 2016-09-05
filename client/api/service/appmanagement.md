## appmanagement

### APIs
| Property      | Parameters    | Return Type   | Description   |
| ------------- | ------------- | ------------- | ------------- |
| installFile | filePath:string, appId:string | result:boolean | install app from local path (path from downloadinfo) |
| installURL | url:string, appId:string | result:boolean | install app from remote url |
| scan | void | void | refresh installed apps |
| remove | appId:string, removeAll:boolean(optional) | result:boolean | remove app, if not removeAll, app data will not be removed. |
| list | category:string | sandboxs:EOSList | list apps by category |
| pathForApp | appId:string | path:string | return app's absolute path by appId |
| getAppSandbox | appId:string | sandbox:AppSandbox | return the sandbox by appId |
| getPageSandbox | appId:string, pageId:string(optional) | sandbox:PageSandbox | get page sandbox by appId and pageId, if pageId was not set, return the page sandbox of the default page. |
