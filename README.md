### SonarQube

In the Project folder Run the next command to install using docker compose

sudo docker-compose -f sonarqube.yaml up -d


After it finish pulling the image and starting open a web browser enter into:

localhost:9000

## Log in
Log in using admin as both user and password, then change the password

## Create Project

Select create Project then fullfil the information, like in the next example

<img width="433" alt="Captura de pantalla 2024-05-14 a la(s) 8 24 28 p  m" src="https://github.com/Estebanm1812/Sonarqub/assets/69942961/614c3d1d-4f77-4914-abee-a763885c9352">

Then select the baseline for new code in the project, in this case we used global setting

<img width="1013" alt="Captura de pantalla 2024-05-14 a la(s) 8 25 28 p  m" src="https://github.com/Estebanm1812/Sonarqub/assets/69942961/c53ed449-f005-4384-82cf-302042bc1596">

### Analysis Method

Selec a Method to analize your code, in this case we will use a local Project

1. generate a token 
<img width="796" alt="Captura de pantalla 2024-05-14 a la(s) 8 33 42 p  m" src="https://github.com/Estebanm1812/Sonarqub/assets/69942961/8586648a-b241-4421-aaa4-a95e0586233a">
2. Save the tokken genereate in the last step and click in continue
3. Select the option that fits the most to your project

<img width="796" alt="Captura de pantalla 2024-05-14 a la(s) 8 35 36 p  m" src="https://github.com/Estebanm1812/Sonarqub/assets/69942961/2d6b70c2-e363-47e6-8d50-2d303b409c11">

in this case we are going to choose "Other" and the Operative System,in this case macOS
4. we install de sonarqub commands using homebrew
brew install sonar-scanner
5. then run the following command in our project's folder

<img width="1345" alt="Captura de pantalla 2024-05-14 a la(s) 8 39 17 p  m" src="https://github.com/Estebanm1812/Sonarqub/assets/69942961/10199a39-ce5a-4a07-876a-181325182c96">

6. After it finish analyzing the page of sonar refresh and give you the data
   
<img width="1415" alt="Captura de pantalla 2024-05-14 a la(s) 9 10 14 p  m" src="https://github.com/Estebanm1812/Sonarqub/assets/69942961/df409c3a-08a4-4f8a-91f9-20a7ea547a7c">

in this we can see there is security problem, if the click it give us more information

<img width="888" alt="Captura de pantalla 2024-05-14 a la(s) 9 12 16 p  m" src="https://github.com/Estebanm1812/Sonarqub/assets/69942961/1ac16ea2-3a78-461a-8130-cf53c9504bba">

in the previus image you can see that sonarqube shows where is the problem and how to fix it

<img width="888" alt="Captura de pantalla 2024-05-14 a la(s) 9 13 08 p  m" src="https://github.com/Estebanm1812/Sonarqub/assets/69942961/17d50cef-43c9-4cea-ad69-c34ff5036419">

Along with more useful information
