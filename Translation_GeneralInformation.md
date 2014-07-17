Translation/Localization: General Information (Version 3.1)
***

The idea of this chapter is to give you some insides into translation and localization of GoldenCheetah. And the relation between a language configured in GoldenCheetah, the behaviour of the development environment which is used to implement GoldenCheetah and the language configured in the underlying operating system (like Window, MacOS or Linux.)

_Note: If you run GoldenCheetah on an operating system configured in "english" (System-Locale), and also configure GoldenCheetah to use "english" as UI language, there is not need to read through this chapter. Everything will work as you expect from a UI language perspective._

Translation/Localization of software is a huge topic. GoldenCheetah has been available in a version which allows the selection of your preferred UI language since a few version - and most of the UI is translated. Still - with new features coming out - also the translation has to enhanced to cover those new features. So it's an ongoing process to keep the software translated.

Let's look into some details:

* Translation - is the availability of the User Interface (UI) in more than one language. Ususally software is developed with UI (screen texts,...) in one language. Development tools usually offer the ability to prepare the UI for a later translation. With these tools, texts can be translated and the UI appears in a different language. 

_Note: Important is, that mostly the translation process is decoupled from development. So a translator does not see the texts he/she is translating in the context of screens / UI elements. The development environment GoldenCheetah is using, also works this way. Dis-advantage of such an translation approach is that specific language testing is required to ensure correct context specific terminology. (Why - many terms demand different translation based on context.)_

* Localization - is the ability of software handle region or country specific requirements. (Easy to understand in business software (e.g. taxation rules,...). Luckily this does not to much effect GoldenCheetah. But still there are some example. Most popular is the representation of 'Dates' and 'Time' in different regions and/or languages. 

With these (maybe boring) explanations - now the specifics for GoldenCheetah:

### Specifics for GoldenCheetah

* GoldenCheetah vs. your operating system language - depending on your operating system language and the language you have configured in GoldenCheetah you might face a UI being presented in two languages. Your OS language and the GoldenCheetah language you have setup in preferences. This is NOT an error in GoldenCheetah, but is caused by the behaviour of the development framework GoldenCheetah is using in combination and the operarating system. E.g. when using a 'File Chooser' dialog in Windows 7 in a setup where only 'English' is the language installed in Windows, the standard dialog features will come up in english, the dialog box nme and any configurable parts of the dialog box will come up in the language you have configured in the GoldenCheetah preferences.

* Change of Language - when changing the language in GoldenCheetah preferences this change takes only effect after closing and restarting GoldenCheetah.

_Note: The change does not only change the 'fix' UI texts in GoldenCheetah, but also initiates the translation of 'Chart' names and ........_

* Date / Time representation - is handled in different ways starting with versio 3.1  DATES shown on screens are subject to localisation. So they are formatted following the rules of the language configured in GoldenCheetah preferences (assuming translation is completely done for that language). TIME is not localized any more, but always presented in the international format 'hh:mm:ss' without any AM/PM formatting.

_Note: Please be aware that the development framework may create some unexpected behavior if system language is different to GoldenCheetah preferences language. E.g. the day and months names and their abbreviations used in the dates diplayed are using the system locale of the operating system, not the language setup in GoldenCheetah preferences._

BACK: [Table on contents] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Main-Page_Table-of-contents)