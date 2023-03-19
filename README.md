# fact_of_image

<strong>this a research about the fact of a Container image <strong> <br>

Objectifs : 
* what is an image in the fact 
* is image just a executable code so what is the relationship between a code and blob (Binary Large OBject) that is a type of unstructed data 

so First things First , we gonna introduce some definitions so we can be sure that we all in the same page 
 
# <strong> what is a Container image : </strong><br>
When running a container, it uses an isolated filesystem. This custom filesystem is provided by a container image. Since the image contains the container’s filesystem, it must contain everything needed to run an application - all dependencies, configurations, scripts, binaries, etc. The image also contains other configuration for the container, such as environment variables, a default command to run, and other metadata.<br>
<italic> if you don't really understand  the definition don't worry u  gonna understand it later in this article because this is the point of this research understanding the fact of an image  </italic>

# <strong> what is a blob : </strong><br>
The term "blob" is short for "Binary Large OBject," which is a common term in computer science that is a type for a large piece of data that is stored in a database or other data structure. 

# <strong> what is unstructered and structered  data : </strong><br>  
Structured data is highly specific and is stored in a predefined format like Number , varchar() , where unstructured data is a conglomeration of many varied types of data that are stored in their native formats 

now if we want to download an image : <br> 

              podman pull <path_of_image> 
             
so we gonna have this result : 

![WhatsApp Image 2023-03-19 at 12 46 36](https://user-images.githubusercontent.com/100031609/226173393-eccc5191-4fc9-4591-8594-266c11d149db.jpeg)

as we see that the container has been build on tree layer each blob is a layer 

because if we do 

              podman inspect <path_of_image> 
              

 we gonna see : <br> 
 
 ![WhatsApp Image 2023-03-19 at 13 06 54](https://user-images.githubusercontent.com/100031609/226175040-d8f966bb-ccc6-4176-8071-b2e4df11e8ba.jpeg)<br>
 
 so this containers is build on three layers and every layer is called a blob so this is the point of our research why the called a blob  <br> 
 
 ![WhatsApp Image 2023-03-19 at 13 06 54](https://user-images.githubusercontent.com/100031609/226174414-57978a4c-b28c-41f3-8a64-a56936458f24.jpeg) 
 <br> 
 
 as we see that every layer is in base64 format  <br>
 so now we are certain that these executables files  are stored as blob type 
 
 so i thing they called the executable code  as an image because is stored in the database as they store true images (like Profile_image ) in the database 
 
 and they store data in blob cells because of their (blobs) flexibility and ability to handle large volumes of data. 
 
 Note :   <br> 
 Containers contains all necessary things ( dependencies , code , Apis .... ) to make the project run seccusfully so this is why containers are heavy 
 
<br>
 
 
<strong>some Common examples of files stored in a BLOB data type field include:<strong>

* Images (JPG, JPEG, PNG, GIF, HEIC, WEBP, raw binary data)
* Videos (MP4, AVI, MOV, MKV)
* Audio files (MP3, WAV, AAC)
* Documents (PDF, TXT, CSV, DOCX, XLSX)
* Archives (ZIP, RAR)
* Executable files (EXE, MSI)
* Backups (SQL, BAK)

Summary : 
  * that an image is a set of all dependecies , script , configuration ....
  * all dependecies , scripts , configuration ... called Container fileSystem 
  * they call container image because they store container filesystem as they store real images with blob type 
  * container image has a blob type because they are heavy and for other reasons as we see before 
  
 
 
