##Onboard New Users onto a Linux Server.

#Created and named the shell script Onboarding_Users.

![shell1](https://user-images.githubusercontent.com/94229949/175724179-dfa1a867-5866-41b2-a776-b0a45db8fa88.png)

![shell 2](https://user-images.githubusercontent.com/94229949/175724355-69887ae6-5146-49dd-99c9-3e00ac7a4c24.png)

![today vs 2](https://user-images.githubusercontent.com/94229949/175725708-67e282de-3e81-4aca-83b8-8d38117779a8.png)

![today vs 3](https://user-images.githubusercontent.com/94229949/175725902-a9c02a9e-bbb6-4a65-be86-5c3ff1768ead.png)

##The script is able to read from the CSV file ,create each user on the server, and add to an existing group called developers.User created also has a default home folder,has a .ssh folder within its HOME folder and an authorized_keys file which has the public key.

##Spinned up an Ubuntu Server on AWS.

![shell 3](https://user-images.githubusercontent.com/94229949/175733941-88c2069c-c3dd-47cd-88b3-6e8448308ec1.png)

##Copied the file Onboarding_users to Ubuntu server using the SCP command.

![today vs 4](https://user-images.githubusercontent.com/94229949/175743742-3a746b6f-3307-41ac-a89c-8edb4ff1f6db.png)

##I then SSH into the AWS Ubuntu Server

![today vs 5](https://user-images.githubusercontent.com/94229949/175749567-88eaabc2-2729-40be-80b8-108b96adc6d5.png)

##created a directory called Shell and moved Onboarding_users to Shell directory.

##Created files ' names.csv ' , ' id_rsa ' , ' id_rsa.pub ' using  ' touch ' command.

##Private key was copied to the file ' id_rsa ' and public key was copied to the file ' id_rsa.pub '

##Names were entered into ' names.csv ', which the script would utilize to generate new users. 

![today vs 8](https://user-images.githubusercontent.com/94229949/175747241-15c6ba36-1274-4338-bb78-c97c89d8e90f.png)

##Created a group called developers where all new users will be added to using the ' groupadd ' command.

##Changed permission on the Onboarding_Users file using ' chmod +x ' command 

##Ran the Shell Script 

![today vs 9](https://user-images.githubusercontent.com/94229949/175748711-26b5200e-8bfe-4708-96b7-058f7d18a491.png)

##Switched User to Root to onboard new users onto the server

![yeeemi](https://user-images.githubusercontent.com/94229949/175748851-c14fee30-c061-4cc9-b6d4-89a10180cfc2.png)

![yeemi1](https://user-images.githubusercontent.com/94229949/175748887-dd23ef78-0f4d-417d-aac1-a07764f213a3.png)

##To check if the new users has been created from ' names.csv ' file ,i ran ' ls -l /home/ ' command 


![today vs 11](https://user-images.githubusercontent.com/94229949/175749142-a882e5fe-22ca-44e0-952b-0ea713889650.png)

##Checked if the authorized_keys file and.ssh file were created with the appropriate permissions and the public key was successfully stored in the authorized_keys file.

![bb1](https://user-images.githubusercontent.com/94229949/175750872-7b5a6f63-ed7b-4aa9-ba22-12f9d43513bc.png)


![bb2](https://user-images.githubusercontent.com/94229949/175750882-234ab5c0-0746-49fa-a1cf-be012893cdae.png)

##To log in as the new user i copied the private key to a file called yemi.pem on my local machine.

##SSH using the private key and the name of the new generated user.

##Logged in as @gbadero

![today vs 12 1](https://user-images.githubusercontent.com/94229949/175749643-20faf256-ce1c-48c4-b0cd-31beb7aaaf33.png)

##Logged in as @busola

![today vs 12](https://user-images.githubusercontent.com/94229949/175749685-280cb18b-f58b-4b7e-80fb-03ad12a8e7ad.png)

