# SF-Custom-Settings-Exporter
CustomSettingsExporter is a class which allows you to export **VALUES** of custom settings from one org to another (ex. from developers Sandbox to full sandbox or Production).
CustomSettingsExporter picks every value of specified custom setting, creates a code, which you can *paste and launch right away*, which inserts a list of custom settings.
To work properly, custom settings devnames on FROM-org must be the same as on TO-org.

Custom settings will be sent to you in a corresponding email.

To start an exporting custom settings see the methods below:

- **addCS(*String* or *SObject*)** - adds a CustomSetting for exporting (ex. *addCS('myCS__c');* or *addCS(new MyCS__c())*).
- **clearCS()** - clears the list of custom settings to export.
- **exportCS(*empty* or *String* or *Id*)** - When left ***empty*** - sends an email to currently logged user. When an ***Id*** is provided - sends and email to specified Lead, Contact or User. When ***String*** is provided - sends and email to specified email address.

*Custom settings are sent ready to be inserted in the console and launched.*
