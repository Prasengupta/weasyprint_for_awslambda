                                   

 <h1>Supporting WeasyPrint in AWS Lambda</h1>
WeasyPrint is a visual rendering engine for HTML and CSS that can export to PDF. It aims to support web standards for printing. WeasyPrint is free software made available under a BSD license.

 * Website: http://weasyprint.org/
 * Latest documentation: http://weasyprint.org/docs/
 * Source code and issue tracker: https://github.com/Kozea/WeasyPrint

The above source code works in windows machines but this library will not work in AWS lambda because of Operating system compatibility. So we have leveraged the library to support in AWS Lambda including few other related files from centOS and generated a working library for AWS lambda.

<h4>How it works in AWS Lambda ?</h4>

<b>Step 1:</b> Download the zip file from this repository. <br>
<b>Step 2:</b> Include your main handler file in the folder and zip it, upload the zip folder to aws lambda. Make sure that the runtime is set as Python 2.7

NOTE: This package doesn't work in windows operating system as it is a lambda package where the lambada runs on centOS
