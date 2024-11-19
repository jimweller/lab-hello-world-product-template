# Hello World Product

This is a very simple C# project that developers can use to get a Hello World
application running in a Windows EC2 VM in AWS.

The intent is that the developer does not need to know about AWS or terraform internals.
They commit code and RDP to a Windows server to see the results.

This is part of [a suite of
repositories](https://github.com/jimweller?tab=repositories&q=hello-world&type=&language=&sort=)
that work together to help new developers get up to speed quickly with a .NET
`Hello World` console app running on a Windows EC2 in AWS.

## Usage

1. Fork the product repository to your own repository in the `ExampleCoDept` org
2. `git clone` the repository locally
3. Edit `Program.cs` and change the "Hello World" string to something new
4. `git commit` and `git push` the code back to remote
5. Go to your fork in github.com
6. Go to actions
7. Acknowledge that you want to use the workflows in the fork
8. Click `Hello AWS` on the left
9. Click run workflow on the left, wait for it to complete
10. Login to AWS (`SEU Sandbox` account as of this writing)
11. Go to S3 -> fcc-demo-hello-world-artifacts and see your zip file
12. Go to EC2 and see your fcc-demo-hello-world-NAME ec2
13. Select your ec2 and click connect
14. Click connect to get a command line
15. Type `c:\hello\hello.exe` to run your code
16. Back in github, run the `Goodbye AWS` action to cleanup. DO THIS OR YOU WASTE MONEY!
17. [Optional] Archive your repo fork
