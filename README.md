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
 
 
