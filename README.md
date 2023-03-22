# fact_of_Container_image




Objectifs : 
* what is an image in the fact 
* is image just a executable code so what is the relationship between a code and blob (Binary Large OBject) that is a type of unstructed data 
* why they call it image 

>so First things First , we gonna introduce some definitions so we can be sure that we are all in the same page 
 
# <strong> what is a Container image : </strong><br>
When running a container, it uses an isolated filesystem. This custom filesystem is provided by a container image. Since the image contains the container’s filesystem, it must contain everything needed to run an application - all dependencies, configurations, scripts, binaries, etc. The image also contains other configuration for the container, such as environment variables, a default command to run, and other metadata.<br>
>if you don't really understand  the definition don't worry u  gonna understand it later in this article because this is the point of this research understanding the fact of an image  

# <strong> what is a blob : </strong><br>
The term "blob" is short for "Binary Large OBject," which is a common term in computer science that is a type for a large piece of data that is stored in a database or other data structure. 

# <strong> what is unstructered and structered  data : </strong><br>  
Structured data is highly specific and is stored in a predefined format like Number , varchar() , where unstructured data is a conglomeration of many varied types of data that are stored in their native formats. 
 
 
## Let's go to the terminal to see what happen 

i utilize podman instead of docker but is the same logique <br>
 
now if we want to download an image : <br> 


              podman pull <path_of_image> 
             
so we gonna have this result : 

![WhatsApp Image 2023-03-19 at 12 46 36](https://user-images.githubusercontent.com/100031609/226173393-eccc5191-4fc9-4591-8594-266c11d149db.jpeg)

as we see that the container has been build on three layers each blob is a layer 

because if we do 

               podman inspect <path_of_image> 
              

 we gonna see : <br> 
 
 ![WhatsApp Image 2023-03-19 at 13 06 54](https://user-images.githubusercontent.com/100031609/226175040-d8f966bb-ccc6-4176-8071-b2e4df11e8ba.jpeg)<br>
 
 so this containers is build on three layers and every layer is called a blob so why they call a layer a blob  <br> 
 
 ![WhatsApp Image 2023-03-19 at 13 06 54](https://user-images.githubusercontent.com/100031609/226174414-57978a4c-b28c-41f3-8a64-a56936458f24.jpeg) 
 <br> 
 
 as we see that every layer is in  [base64](https://en.wikipedia.org/wiki/Base64) format  <br>
 
 
 so now we are certain that those layers are stored as blob type
 
 this is  why when we want to download the image we see that those layers named blobs  to tell as that those layers are stored with a blob type 
 
 layers contains dependencies , configurations, scripts ... and each modification of the image commited make a new layer 
 
 
 and they store data in blob cells because of their  flexibility and ability to handle large volumes of data. 
 
 Note :   <br> 
 Containers contains all necessary things ( dependencies , code , Apis .... ) in layers to make the project run seccussfully so this is why layers are heavy 
 
<br>
 
 
<!-- <strong>some Common examples of files stored in a BLOB data type field include:<strong>

* Images (JPG, JPEG, PNG, GIF, HEIC, WEBP, raw binary data)
* Videos (MP4, AVI, MOV, MKV)
* Audio files (MP3, WAV, AAC)
* Documents (PDF, TXT, CSV, DOCX, XLSX)
* Archives (ZIP, RAR)
* Executable files (EXE, MSI)
* Backups (SQL, BAK)
-->
Summary : 
  * a Container image is a groupe of layers that contain dependencies ,  script , configuration .... in an organized way 
  * image is build in three layers each layer stored with a blob type this is why they call each layer a blob when we pull it from the database (image regestry)
  * Image layer has a blob type because they are heavy and for other reasons as we see before 
  * they call image because in the fact is a group of layers that is in the fact group of blobs and a group of blobs is a blob (TY5UN(blob) + IOK4(blob) = FRGO(blob))    the result is a blob so logicaly an image 
  
 
 
