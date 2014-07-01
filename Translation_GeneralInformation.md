Translation/Localization: General Information (Version 3.1)
***

The idea of this chapter is to give you some insides into translation and localization of GoldenCheetah. And the relation between a language configured in GoldenCheetah, the behaviour of the development environment which is used to implement GoldenCheetah and the language configured in the underlying operating system (like Window, MacOS or Linux.)

_Note: If you run GoldenCheetah on an operating system configured in "english" (System-Locale), and also configure GoldenCheetah to use "english" as UI language, there is not need to read through this chapter. Everything will work as you expect for a UI language perspective._

Translation/Localization of software is a huge topic. GoldenCheetah has been available in a version which allows the selection of your preferred UI language since a few version - and most of the UI is translated. Still - with new features coming out - also the translation has to enhanced to cover those new features. So it's an ongoing process to keep the software translated.

Let's look into some details:

* Translation - is the availability of the User Interface (UI) in more than one language. Ususally software is developed with UI (screen texts,...) in one language. Development tools usually offer the ability to prepare the UI for a later translation. With these tools, texts can be translated and the UI appears in a different language. 

_Note: Important is, that mostly the translation process is decoupled from development. So a translator does not see the texts he/she is translating in the context of screens / UI elements. The development environment GoldenCheetah is using, also works this way. Dis-advantage of such an translation approach is that specific language testing is required to ensure correct context specific terminology. (Why - many terms demand different translation based on context.)_

* Localization - is the ability of software handle region or country specific requirements. (Easy to understand in business software (e.g. taxation rules,...). Luckily this does not to much effect GoldenCheetah. But still there are some example. Most popular is the representation of 'Dates' and 'Time' in different regions and/or languages. 

With these (maybe boring) explanations - now the specifics for GoldenCheetah:

### Specifics for GoldenCheetah

* GoldenCheetah vs. your operating system language

* Change of Language

* Date / Time representation

* Dynamic Translation of Charts

