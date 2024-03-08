
# Android Component for Conversion and Formatting Functions

This library contains various functions for formatting a particular date from one format to another format like "yyyy-MM-dd'T'HH:mm:ss'Z'" format to “dd MMM yyyy h:mm a” format etc. This library also contains functions to convert a particular string to base64 format and convert base64 format to string. Base64 format generally used in encrypting any string. It can also be used to validate any password and any characters which should contain lowercase letters, uppercase letters, digits, underscores, and spaces etc. 





### Deployment

To get a Git project into your build:

#### Step 1. Add the JitPack repository to your build file

Add it in your root build.gradle at the end of repositories:

```bash
  dependencyResolutionManagement {
		repositoriesMode.set(RepositoriesMode.FAIL_ON_PROJECT_REPOS)
		repositories {
			mavenCentral()
			maven { url 'https://jitpack.io' }
		}
	}
```

#### Step 2. Add the dependency

```bash
dependencies {
	        implementation 'com.github.nayanapetkar2024:conversionformattingfunc:2.16'
}

```

### Importent things to remember

 To use this library we have to make sure that minSDK of app level and module level build.gradle set to 24.


### Description about the functions 

This library contains 12 functions.

    1. convertStringToBase64(String anyString) 

        This function returns Base64 encryted string. 
        This function can be use to convert any String to Base64 encrypted format.

    2. convertBase64ToString(String Base64)

        This function returns String. 
        This function can be used to convert any Base64 encrypted string into string format.

    3. isValidPassword(String anyString)
        
        This function return boolean .
        This function can be use to check password validation ex. First letter should be caps, it should have atleast one special character and numeric. 
        If the password pass the validity check then it will return true else false.

    4. getCurrentDateYMD()

        This function return current date in "yyyy-MM-dd" format in string format.

    5. getFormattedDateDMYHMA(String date)

        This function return date in below format in string format:

                Input date format:  "MM/dd/yyyy h:mm a"
                Output date format: "dd MMM yyyy h:mm a"


    6. getFormattedDateYMD(String date)

        This function return date in below format which is in string format:

                Input date format:  "dd MMM yyyy h:mm a"
                Output date format: "yyyy-MM-dd"

    7. getFormattedDateToStringFormat()

        This function return date in"yyyy-MM-dd'T'HH:mm:ss'Z'" format in string format.

    8. getFormattedDateDMYHMADateZone(String date)

        This function return date in below format which is in string format:

                Input date format:  ""yyyy-MM-dd'T'HH:mm:ss'Z'"
                Output date format: "dd MMM yyyy h:mm a"

    9. getFormattedStringDateToDateFormat(String dateInStringFormat) 

        This function return date in below format which is in date format:
                Input date format:  "yyyy-MM-dd'T'HH:mm:ss'Z'"
                Output date format: "EEE MMM dd HH:mm:ss zzz yyyy"

    10. formatMobileNumber(String mobileNumber)         

        This function return mobileNumber in International US format.

    11. formatToDecimal(String amount)

        This function return string integer with two decimal format ex. 5.00

    12. isValidChar(String anyString)
        
        This function return boolean.
        This function can be use to check character validation which should contain lowercase letters, uppercase letters, digits, underscores, and spaces.
        If the character pass the validity check then it will return true else false. 
