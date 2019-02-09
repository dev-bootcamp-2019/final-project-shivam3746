# Certificate Issuer

This decentralized application is able to issue a particular certificate to the holder on the blockchain network upon completing a course upto a certain level.
Issuing certificate on the blockchain network will make this credential remain forever registered with the holder's unique address which can further be used to verify the originality of the certification credential.

This dapp is properly deployed on Ropsten Test Network for the test purpose and it was running fine on the server _localhost//:3000_
Screenshots are provided for better observations.

## User Story

So, Ramesh is a front-end developer by profession , one day he decided to upgrade his skills and he took some time and took an online course on blockchain .Upon successful completion of the course Ramesh received
a certificate from the organisation but the organisation offered two ways to receive credential in which he had to opt one.
1. Receive a pdf of the ceritificate.
2. Receive your certificate on the blockchain network.

Ramesh made a smart move by opting the second option as in this he has not to worry about his authneticity with the credential 
He has not to worry about where to safely store the credential.As Credential is forever registered on the blockchain network.

### Dependencies

Make sure to install npm, webpack, webpack-cli globally.

```npm install```

```npm install --save-dev webpack```

```npm install --save-dev webpack-cli```

### Deployment

1. Login your Meta Mask Account
2. Go to the project directory and run ```npm run start``` in the terminal.
3. Select the Ropsten Network in MetaMask.

#### Note-:
This project has also some essential files for integrating uPort(a ownership identity verification dapp) but currently this project is missing functionality of integration with uport as i have plans to integrate it further to allow the usage of this certificate issuing dapp at a wide scope with one time identity verification with push notifications regarding the alerts for the credential issued.

### Interaction

Once the application starts on the localhost you have to interact with the contract phase and for this you shoul follow some input guidelines
1.Below the Name field , try to input only string value i.e. "Your Name"
2.Below the Level field try to input only integer values i.e. from 0-9 but it has got some conditions
    I-:Your metamask transaction will be failed if you will input the integer value above "3" because certifcates will be assigned on          only level 1,2 and 3.
   II-:You will be assigned with the certificate on the blockchain network by confirming metamask transcation successfully if you              provided the level between 1-3. 
