# fact_of_image

<strong>this a research about the fact of an image <strong> <br>

Objectifs : 
* what is an image in the fact 
* is image just a executable code so what is the relationship between a code and blob (Binary Large OBject) that is a variable of images  

so First things First , we gonna introduce some definitions so we can be sure that we all in the same pages 
 
![Screenshot (91)](https://user-images.githubusercontent.com/100031609/226125425-2d320df7-d503-44d2-9941-7db69bb4ca0d.png)

so now what is a blob : <br>
The term "blob" is short for "binary large object," which is a common term in computer science for a large piece of data that is stored in a database or other data structure. 

now if we want to download an image : <br> 

              podman pull <path_of_image> 
             
so we gonna have this result : 

![WhatsApp Image 2023-03-19 at 12 46 36](https://user-images.githubusercontent.com/100031609/226173393-eccc5191-4fc9-4591-8594-266c11d149db.jpeg)

as we see that the container has been build on tree layer each blob is a layer 

because if we do 

              podman inspect <path_of_image> 
              

 
