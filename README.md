# Trabajo-1-trimestre.-Servidores-web

![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/ea5ce249-cac7-4e57-8324-e56b80feffb4)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/cda2182e-d690-43f0-8788-2b28d30f061b)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/e8bdf262-6084-4ca1-a31b-6d0bf1510e49)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/c5c27d1c-201d-4f2f-af6b-ac8445d097b1)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/e1976c34-3448-447a-8103-10de61e784fc)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/94cdbc58-f60e-4ede-af46-3a0141c2f8bf)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/30d93869-474c-4513-b958-b430e302e70b)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/e235e5e9-466f-45bf-b9a0-5d9e95f4ad02)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/a84c1c9e-3a2e-49a8-af0a-b8d5fecb6fd5)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/49b3190f-3e01-43c2-badf-8069d7c04793)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/c0de91c4-8139-4faa-b170-e894c96026e8)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/6ea3c17a-ee17-42ec-a3ed-3c47517126b8)
Ya podemos comprobar desde el browser con localhost/index.php y nos sale esta pagina:
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/40103438-85b4-47f9-8174-eb624a3aa56e)
Instalamos el paquete mysql-server
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/32c0c60f-ca66-4b5f-b8b5-311d252ba5e2)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/3422f02a-34f4-44fe-8f8e-1b35df3470da)
ls -l /var/www/html
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/0026539c-8df9-49a1-b6b0-b89a4be09f55)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/c370aad0-a5c5-4d1a-9884-739ee33491a8)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/6b71fa86-f17a-4565-abc8-1f8e5640a0d6)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/29928675-42bb-4348-b645-6bb1b6cf7b8a)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/9918d753-4e16-4a9b-ad78-f922678433ab)
Finalmente instalamos PHP y sus complementos con el siguiente comando:
sudo apt install php libapache2-mod-php php-mysql
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/18f757a7-c9b6-406e-86df-36f4db48a5a6)
Ahora tiene una base de datos y una cuenta de usuario, creadas específicamente para
WordPress. Debemos eliminar los privilegios de modo que la instancia actual de MySQL
sepa sobre los cambios recientes que hemos realizado
Cierre MySQL escribiendo lo siguiente: exit
Iniciar apache2 con el comando: sudo systemctl restart apache2. También muy importante
cambiar este fichero:
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/f09ddfc3-f8ca-4e5b-a329-50498b535af6)
Debemos ir a las siguientes líneas: y cambiamos lo siguiente
● DB_NAME wordpress
● DB_USER usuario
● DB_PASSWORD usuario
Establecemos el nombre y contraseña creados en la base de datos:
Ahora para crear host virtual de Apache para el sitio web de WordPress, se requiere
configurar el servidor web Apache para que aloje el sitio de WordPress con el nombre de
dominio.
Para ello debemos crear un host virtual y establecer la configuración de Apache, ejecutamos
lo siguiente:
sudo nano /etc/apache2/sites-available/centro.intranet.conf
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/a440aeb3-f0a5-4bbf-92ef-abb4c42f5bc2)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/e37f4b5c-9f18-4cfa-ba63-5d67778b1386)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/c4adabc2-c7fe-42a2-b6ca-74982b227523)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/bc998e00-91b6-46db-8ac7-1775bb6942c5)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/629d1c9a-a77a-4cc1-86cd-5d3199d3db69)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/461bedc5-99ff-4f0f-8056-a06cef041e79)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/c77556f9-298e-4260-b2a3-4d387d11c014)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/f96fbcb9-4e04-4bac-b6fa-0ee055cf0901)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/1a32b202-de52-41cd-902a-f227eb30b750)
Ajustar la configuración de Apache para permitir anulaciones y reescrituras de .htaccess
Habilitar anulaciones de .htaccess
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/8e1b5057-4029-41bc-81d1-fb58653092ad)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/12890ce6-3611-47b6-a943-6c4b3eeefd78)
A continuación, abrimos el archivo de configuración de WordPress: cambiamos “pon aquí tu
frase única” con lo siguiente
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/20da8e7c-a220-4511-bf7b-3c9561d35444)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/1f3e7c11-89a2-4844-86bb-a334e98431ce)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/773fff34-60c4-421d-b028-cb8f126b8176)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/40a8f9c3-969a-4eb1-9b00-7c181e11b37d)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/31e6f31c-399f-4fdd-b7fe-b7c5a5a5b0d5)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/4f6b3cdb-5c7d-4664-a09e-95405ae32d39)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/f156858e-0f73-49b3-b076-bd89e0e2775b)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/1544e847-a5f2-40c4-9ef8-e2d9c6820bc9)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/2fd3febd-c48e-4dcf-a035-4bfad3198e01)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/d82437ae-b54e-44d8-b325-69f6499ab196)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/f2656dbe-7165-483b-9c3e-5e7b6ce071bc)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/1e4d0b89-49d0-4f74-b8e8-c06a4b8e886c)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/0f8476af-27f7-4d34-903b-9c9b1140028c)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/df3491fd-3c66-4c02-b4b6-cee1cb929bfa)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/89ac3470-65b6-4aa6-b664-785730a4eac7)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/bd0b1c52-8961-476f-975d-622f68c5bc36)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/55cadfde-c7fb-46de-b3ba-7672caf47cfe)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/d6ce4fca-4236-4d9d-b206-f650d4b3ca23)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/ac459aef-206a-4ac2-b162-dd36892a66a5)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/52a92520-3260-4d7f-9473-87b630495726)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/7fa0d0a4-a150-44ac-9da9-229eab3f48ea)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/8edde891-b2a3-434e-b085-d285200122d2)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/496987e8-fc4e-4a73-a1cd-482aff272b18)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/a3c9145c-7e70-4c68-96e9-4a819d0ba43e)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/8fa5f7b2-8a0f-4b4e-b612-68d496e4918a)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/35c04c4e-fbf2-4e90-9245-cee4fe8c7f72)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/36c563db-e920-435e-9b65-809ff142a422)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/bf3f2d90-f134-44ba-abb6-e27a9e9adc49)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/3e4ca1ce-2425-411a-8bbc-785b6deddbca)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/dfbcd40b-d411-4d46-bb60-d88f915977f3)
![image](https://github.com/hasna2223/Trabajo-1-trimestre.-Servidores-web/assets/119622209/5cb84c3d-27ff-47ee-a285-0ea1726480d5)
