Translation/Localization: General Information (Version 3.1)
***

The idea of this chapter is to give you some insides into translation and localization of GoldenCheetah, as well as the relation between a language configured in GoldenCheetah, the behavior of the development environment which is used to implement GoldenCheetah and the language configured in the underlying operating system (like Window, MacOS or Linux.)

_Note: If you run GoldenCheetah on an operating system configured in "english" (System-Locale), and also configure GoldenCheetah to use "english" as UI language, there is not need to read further. Everything will work as you expect from a UI language perspective._

Translation/Localization of software is a huge topic. GoldenCheetah has been available in a version which allows the selection of your preferred UI language since a few versions - and most of the UI is translated. Still - with new features coming out - also the translation has to enhanced to cover those new features. So it's an ongoing process to keep the software translated.

Let's look into some details:

* Translation: Is the availability of the User Interface (UI) in more than one language. Usually software is developed with UI (screen texts,...) in one language. Most development tools offer functions to prepare the UI for a later translation. With these tools, texts can be translated and the UI can switch to a different language. 

_Note: Important to understand is, that in most cases the translation process is decoupled from development. So a translator does not see the texts he/she is translating in the context of screens / UI elements. The development environment GoldenCheetah is using also works this way. Dis-advantage of such an translation approach is that specific language testing is required to ensure correct context specific terminology. (Since some terms/texts demand different translation based on context.)_

* Localization: Is the ability of software to handle region or country specific requirements. (Easy to understand in business software (e.g. taxation rules,...). Luckily there is not much need for localization in GoldenCheetah. But still there are some example. Most popular is the representation of 'Dates' and 'Time' in different regions and/or languages.

### Specifics for GoldenCheetah
After those (maybe boring) explanations - now the specifics for GoldenCheetah:

* GoldenCheetah vs. your operating system language - depending on your operating system language and the language you have configured in GoldenCheetah you might face pieces of the UI being presented in two languages. Screens / dialog box with a mixture of your OS language and the GoldenCheetah preferences language are presented. This is NOT an error in GoldenCheetah, but is caused by the behavior of the development framework GoldenCheetah is using and the operating system. E.g. when using a 'File Chooser' dialog in Windows 7 in a setup where only 'English' is the language installed in Windows, the standard dialog features will come up in English, the dialog box name and any configurable parts of the dialog box will come up in the language you have configured in the GoldenCheetah preferences.

* Change of Language - when changing the language in GoldenCheetah preferences this change takes only effect after closing and restarting GoldenCheetah.

_Note: The change does not only change the 'fix' UI texts in GoldenCheetah, but also initiates the translation of 'Chart' names and preset names/metrics_

* Date / Time representation - is handled in different ways. 
  * DATES shown on screens are subject to localisation. So they are formatted following the rules of the language configured in GoldenCheetah preferences (assuming translation is completely done for that language)
  * From 3.1 on TIME is not localized any more, but always presented in the international format 'hh:mm:ss' without any AM/PM formatting.

_Note: Please be aware that the development framework may create some unexpected behavior if system language is different to GoldenCheetah preferences language. E.g. the day and months names and their abbreviations used in the dates displayed are using the system locale of the operating system, not the language setup in GoldenCheetah preferences. This are not errors, but normal behavior in mixed language installations._

### Country specifics

* [Deutsch / German] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG-310-Translation_German)
* ...

BACK: [Table on contents] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG-310-Main-Page_Table-of-contents)