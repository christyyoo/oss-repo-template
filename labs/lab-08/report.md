## Checkpoint 1: Getting Started  
Screenshot of successful build complete message:
![image](https://user-images.githubusercontent.com/60198697/159137381-4f4e1e4c-41a1-4e40-908e-3d1024c0859d.png)  

## Checkpoint 2: Executing the Tests  
**Find the Nightly and Experimental sections and look at some of the submissions. How can you see what tests were run for a particular submission?**  
You can see what tests were run for a particular submission by looking under the Test header and clicking on the numbers. There should be some tests
that have failed or passed. By clicking on the numbers, we can see the details of the tests that have either passed or failed.  

**Find a submission with errors. Can you see what the error condition was? How does this help you debug the failure?**  
In the Nightly section, the Linux-Gentoo-Sparc32-gcc4.8 build passed 691 tests and had 1 failure. By clicking on the failures, we see that the
RunCMake.CompatibleInterface test failed. The test output implies that the test failed because the result did not match the expected output.
This page shows a lot of useful information to debug the failure because it shows which line the error occurred around and telling the user exactly why it failed.  

**Find a system that is close to your specific configuration in the Nightly, Nightly Expected or one of the Masters sections. How clean is the dashboard?
Are there any errors that you need to be concerned with?**  
The build cmake-windows_vs2022_x64 (https://open.cdash.org/build/7803647) is close to my specific configuration.
The dashboard seems pretty clear and there are no errors that I need to be concerned with.  

**Experimental build:**  
![image](https://user-images.githubusercontent.com/60198697/159138619-de75c375-d88c-49a7-bd36-74bd93899b6b.png)  
![image](https://user-images.githubusercontent.com/60198697/159138627-5e29b1bb-2c85-46b9-bd77-3956bf9c0364.png)  
![image](https://user-images.githubusercontent.com/60198697/159138636-0840bfe3-5131-4963-bbbd-4006db619b89.png)  
![image](https://user-images.githubusercontent.com/60198697/159138648-c0edc53d-b87a-4811-824f-fe5c3838b9d0.png)  
There are no errors.

## Checkpoint 3: Failing/Passing a Test  
![image](https://user-images.githubusercontent.com/60198697/159138876-31cc09c6-ad39-43c8-a59e-177dc45c4c4c.png)  
Through the details of the different tests that were run on this build, I was able to catch the error by looking
at the failed test. Test #26: CMake.Copyright failed, so this is where the error occurred. I just had to change the end
date from 2020 to 2022.
![image](https://user-images.githubusercontent.com/60198697/159139044-46829daa-f98d-440f-8643-0aa36de8c1c0.png)  

## Checkpoint 4: CI/CD
