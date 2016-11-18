# Current Sprint Backlog
_Pending_
######Coding stuff
**Finding current directory path:**
```java
System.getProperty("user.dir");
```

**Finding files of a specific type:**
```java
File folder = new File(System.getProperty("user.dir"));
FilenameFilter xmlFilter = (File dir, String name) ->
	{
		if (name.toLowerCase().endsWith(".xml"))
		{
			return true;
		}
		else
		{
			return false;
		}
	};
	File xmlFiles[] = folder.listFiles(xmlFilter);
```
## Previous Backlogs:
####Nov 15th: XMLGen
**Produce a class that creates \*.xmls in a structure defined by Stephen's Team**

**Return type**: _File_ || (_void_ && write to directory)

**Parameters**: _ArrayList_ of Course Info || _Strings_ provided by Debbie's Team

**Potential Throwable Errors**: _FileNotCreated_.


####Nov 8th: Functional Email
**Produce a _WELL DOCUMENTED_ functional multi-recipient multi-attachment Email class**

**Return type**: _void_

**Parameters**: _ArrayList_ of recipients, _ArrayList_ of attachments (as paths in the local machine), _String_ message.

**Potential Throwable Errors**: _invalidRecipient_, _noConnection_, _FileNotFound_, _messageTooLarge?_.

**See Download below for Email API**

## Resources:
* [Download Apache Commons Email(ACE) jar](http://commons.apache.org/proper/commons-email/download_email.cgi)
* [User Guide for ACE API](http://commons.apache.org/proper/commons-email/userguide.html)
* ~~https://docs.oracle.com/javase/tutorial/jdbc/basics/\~~


###### Stylizing this README
[Getting fancy with the README](https://help.github.com/articles/basic-writing-and-formatting-syntax/)
