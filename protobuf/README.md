# itbelongs-tools
Tools to be used to develop API, App, Server and Co.

## protobuf installation instructions for API development
### Windows
Download protoc-28.2-win64.zip and extract to C:\Program Files\protoc\

Add protoc to the system PATH:
    Right-click This PC > Properties > Advanced system settings > Environment Variables.
    Under System variables, find Path, click Edit, and add the path where you extracted protoc (e.g., C:\protobuf\protoc\bin).

Verify installation: Open the command prompt and run:

    protoc --version

Protobuf usage: change to folder .\itbelongs-api\api-messages and execute

    protoc --proto_path=. --python_out=./../api-python --cpp_out=./../api-cpp --objc_out=./../api-objc *

