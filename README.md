# Oxford Dictionary API Connector for Mendix 
The Oxford Dictionary API Connector allows you to easily integrate the Oxford Dictionary API into your Mendix application. This module provides a convenient way to access Oxford Dictionary API endpoints and retrieve data such as word definitions, synonyms, antonyms, and more.
 
## Prerequisites
Before you begin, you will need:
An APP id and API key from Oxford Dictionary API (https://developer.oxforddictionaries.com/)
 
## Configuration
### To configure the Oxford Dictionary API Connector, follow these steps: 
- Obtain an App Id and App Key from the Oxford Dictionary App.
- Set the App Id to a constant variable named APPID and the App Key to a constant variable named APPKey for authentication.
- The default value for the Oxford Dictionary API Base URL is https://od-api.oxforddictionaries.com/api/v2/ , which is set to a constant variable named BaseURL.
- Add the microflow IVK_OpenDictionaryPage to your navigation. (The landing page will have sample implementations for all the services)
- Run your mendix application and test the Oxford Dictonary API connection. 

## Usage
You can follow these steps: 
- Find the microflow for the service you want to use and add it to your action call. For example, if you want to use the Lemmas service, locate the corresponding microflow under the Lemmas folder and call it as a sub-microflow in your action.
- Create an object for the entity ODRequest with the necessary values for the API call. For instance, if you want to use the Entries service, you need to pass a word with a source language as input, set the value to the corresponding attributes, and pass the object as input to the microflow call.
- You can store the response from the API call using Import Mapping created for each service.

You can find the information on supported languages here: https://developer.oxforddictionaries.com/documentation/languages

Future release of this module is planned for:
- Pronunciation play
- Customized selection for grammatical, lexical, domain, register information

##Support
If you encounter any issues or have questions about the Oxford Dictionary API Connector, please contact the module developer or Mendix support for assistance.

## Screenshots
 ![image](https://user-images.githubusercontent.com/46309709/222959922-2491d826-7e2f-4a6e-9330-d7b8fd69c449.png)

 
 

