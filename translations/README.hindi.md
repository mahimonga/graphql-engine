# हसुरा ग्रेफ्लिक इंजन

[[Dokumenti] (https://img.shields.io/badge/docs-v1.0-brightgreen.svg?style=flat)] (https://hasura.io/docs)
[[CircleCI] (https://circleci.com/gh/hasura/graphql-engine.svg?style=shield)] (https://circleci.com/gh/hasura/graphql-engine)


<a href="https://discord.gg/vBPpJkS"> <img src = "https://img.shields.io/badge/chat-discord-brightgreen.svg .logo=discord&style=flat"> </ / एक>
<a href="https://twitter.com/intent/follow?screen_name=HasuraHQ"> <img src = "https://img.shields.io/badge/Follow-HasuraHQ-blue.svg?style=flat&logo = चहचहाना "> </a>
<a href="https://eepurl.com/dBUfJ5"> <img src = "https://img.shields.io/badge/newsletter-subscribe-yellow.svg?style.flat"> </a>

Hasura GraphQL इंजन एक अविश्वसनीय रूप से तेज़ ग्राफक्लाइन सर्वर है जो आपको ** ** webgrook ड्राइवरों **] (../ घटना-triggers.md) के साथ ** वर्तमान,
ग्राफ़िकल एपीआई के माध्यम से पोस्टग्रेज ** प्रदान करता है। डेटाबेस में, और व्यापार तर्क के लिए [** दूरस्थ योजनाओं **] (.. / दूरस्थ-schemas.md)।

Hasura आपको Postgres द्वारा समर्थित GraphQL अनुप्रयोग बनाने में मदद करता है या धीरे-धीरे Postgres का उपयोग करके मौजूदा अनुप्रयोगों के लिए GraphQL पर स्विच करता है।

[Hasura.io] (https://hasura.io) और [दस्तावेजों] (https://hasura.io/docs) पर अधिक पढ़ें।

------------------

![Hasura GraphQL Engine Demo](../assets/demo.gif)

------------------

![Hasura GraphQL Engine Demo u stvarnom vremenu](../assets/realtime.gif)

-------------------

## विशेषताएं

** **मजबूत प्रश्न बनाएं**: अंतर्निहित फ़िल्टरिंग, ब्राउज़िंग, पैटर्न खोज, बैच प्रविष्टि, अद्यतन, म्यूटेशन हटाना
** **वास्तविक समय**: सदस्यता के उपयोग से किसी भी ग्राफक्यूएल क्वेरी को लाइव क्वेरी में परिवर्तित करें
** **दूरस्थ सुदूर स्कीमा** मर्ज करें: एकल ग्राफकॉइल इंजन एंडपॉइंट के माध्यम से कस्टम ग्राफक्यूएल व्यापार तर्क स्कीमाओं तक पहुँचें। [**और पढ़ें**] (../ सुदूर-schemas.md)।
** * वेबकह या सर्वर रहित फ़ंक्शन को समाप्त करें: पोस्टग्रेज के साथ घटनाओं को सहेजें / अपडेट / हटाएं ([और पढ़ें] (.. / इवेंट-triggers.md))
** **मौजूदा, सक्रिय डेटाबेस के साथ काम करता है**: इसे एक मौजूदा पोस्टग्रैज डेटाबेस को निर्देशित करें ताकि ग्राफक्लाइन एपीआई का उपयोग करने के लिए तुरंत तैयार हो जाएं
** * ललित अभिगम नियंत्रण **: डायनेमिक एक्सेस कंट्रोल जो आपके एक्सेस सिस्टम के साथ एकीकृत होता है (उदाहरण के लिए: Andor0, फायरबेस-कोर)
** * उच्च प्रदर्शन और छोटे निशान **: ~ 15 एमबी docker छवि; ~ 50 एमबी रैम @ 1000 अनुरोध / एस; कई कोर
** ** व्यवस्थापक इंटरफ़ेस और माइग्रेशन **: व्यवस्थापक पैनल और रेल-प्रेरित माइग्रेशन योजना
** "पोस्टग्रेट्स ** **: पोस्टग्रैस टाइप्स (पोस्टगिस / जियो-लोकेशन, आदि) का समर्थन करता है, विचारों को * चार्ट्स में कनवर्ट करता है,
म्यूटेशन के साथ संग्रहीत कार्य या प्रक्रियाएं चलाता है।

[Hasura.io] (https://hasura.io) और [दस्तावेजों] (https://hasura.io/docs) पर अधिक पढ़ें।

## विषय - सूची
<! - markdown-toc start - इस अनुभाग को संपादित न करें। एम-एक्स मार्कडाउन-टू-रिफ्रेश-टू-सी -> चलाएं
** विषय - सूची **

- [त्वरित शुरुआत:] (# त्वरित शुरुआत)
    - [हेरोक पर एक-क्लिक कार्यान्वयन] (# कार्यान्वयन-एक-क्लिक-ऑन-हीरो)
    - [अन्य कार्यान्वयन के तरीके] (# अन्य-कार्यान्वयन-तरीके-साथ-एक-क्लिक)
- [वास्तुकला] (# वास्तुकला)
- [ग्राहक उपकरण] (# ग्राहक-पक्ष-उपकरण)
- [व्यापार तर्क जोड़ें] (# ऐड-बिजनेस-लॉजिक)
    - (दूरस्थ योजनाएं) (# दूरस्थ योजनाएं)
    - (डेटाबेस घटनाओं पर रनिंग वेबहूक] (# रन-वेबहूक-ऑन-इवेंट्स-इन-डेटाबेस)
- [डेमो] (# डेमो)
    - (वास्तविक समय के अनुप्रयोग] (# वास्तविक-अनुप्रयोग)
    - [वीडियो] (# वीडियो)
- [सहायता और समस्या निवारण] (# समर्थन - समस्या निवारण)
- [योगदान] (# योगदान)
- (ब्रांडेड सामग्री] (# ब्रांडेड सामग्री)
- [लाइसेंस] (# लाइसेंस)
- [अनुवाद] (# अनुवाद)

<! - markdown-toc end ->

## जल्दी शुरू:

### हेरोक पर एक-क्लिक कार्यान्वयन

हसुरा की कोशिश करने का सबसे तेज़ तरीका हेरोकू है।

1. मुफ्त पोस्टग्रेज प्लगइन के साथ हरोक पर ग्राफकॉक इंजन स्थापित करने के लिए नीचे दिए गए लिंक पर क्लिक करें:

    [! [हरोकू पोस्ट] (https://www.herokucdn.com/deploy/button.svg)] [https://heroku.com/deploy?template=https://github.com/hasura/graphqll इंजन Heroku)

2. हसुरा कंसोल खोलें

   व्यवस्थापक कंसोल को खोलने के लिए `https: // <app-name> .herokuapp.com` (* अपने आवेदन के नाम के साथ \ <ऐप-नाम \> बदलें)।

3. पहले GraphQL क्वेरी बनाओ

   एक स्प्रेडशीट बनाएं और अपनी पहली क्वेरी को तुरंत आज़माएँ। इस [सरल गाइड] (https://hasura.io/docs/1.0/graphql/manual/getting-started/first-graphql-query.html) का पालन करें।

### अन्य एक-क्लिक परिनियोजन विधियाँ

अन्य एक-क्लिक तैनाती विकल्पों के लिए निर्देश देखें:

| ** इंफ्रा प्रदाता ** | ** लिंक ** | ** अतिरिक्त जानकारी **
|:------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------------------------------------------------------------------:|
| DigitalOcean | [[! hasura & utm_campaign = readme) | ]
| Azure | [! [एज़्योर में तैनात] .com% 2fhasura% 2fgraphql- इंजन% 2fmaster% 2finstall- मैनिफ़ेस्ट% 2fazure-container-with-pg% 2fazuredeploy.json) | [डॉक्स] (https://hasura.io/docs/1.0/graphql/manual/guides/deployment/azure-container-instances-postgres.html) |
### अन्य कार्यान्वयन के तरीके

डॉकर-आधारित तैनाती और उन्नत कॉन्फ़िगरेशन के लिए, [कार्यान्वयन गाइड] (https://hasura.io/docs/1.0/graphql/manual/getting-started/index.html) देखें या
[स्थापना प्रकट] (.. / स्थापित-प्रकट)।

## आर्किटेक्चर

Hasura GraphQL इंजन पोस्टग्रेज उदाहरण पर फ्रंट-एंड है और आपके क्लाइंट अनुप्रयोगों से ग्राफकलाइन अनुरोध स्वीकार करता है। यह आपके मौजूदा प्रमाणीकरण प्रणाली का उपयोग करने के लिए कॉन्फ़िगर किया जा सकता है और आपके प्रमाणीकरण प्रणाली के गतिशील चर के साथ क्षेत्र-स्तरीय नियमों का उपयोग करके पहुंच नियंत्रण का प्रबंधन कर सकता है।

आप सुदूर ग्राफकलाइन स्कीमा का विलय भी कर सकते हैं और एक एकीकृत ग्राफकॉल एपीआई भी प्रदान कर सकते हैं।

[[हसुरा ग्रेफ्लिक इंजन आर्किटेक्चर] (.. / संपत्ति / हैसुरा-आर्च.एसवीजी)

## क्लाइंट-साइड टूल

हसुरा किसी भी ग्राफक्यूएल क्लाइंट के साथ काम करता है। हम [अपोलो क्लाइंट] (https://github.com/apollographql/apollo-client) की सलाह देते हैं। [भयानक- graphql] (https://github.com/chentsulin/awesome-graphql) क्लाइंट सूची देखें।

## व्यावसायिक तर्क जोड़ें

GraphQL इंजन आपके बैकएंड में कस्टम बिजनेस लॉजिक जोड़ने के लिए सरल, स्केलेबल और व्यवहार्य तरीके प्रदान करता है:

### दूरस्थ योजनाएँ

कस्टम सॉल्वर को दूरस्थ स्कीमा में हसुरा के पोस्टग्रेज्स-आधारित ग्राफ़कॉल स्कीमा के बगल में जोड़ें। उपयोग के मामलों के लिए आदर्श जैसे कि भुगतान एपीआई के कार्यान्वयन, या आपके डेटाबेस में नहीं डेटा के लिए प्रश्न - [और पढ़ें] (.. / दूरस्थ-schemas.md)।

### डेटाबेस घटनाओं पर एक webhook चलाएँ

डेटाबेस में घटनाओं द्वारा ट्रिगर किया गया अतुल्यकालिक व्यापार तर्क जोड़ें।
सूचनाओं के लिए आदर्श, पोस्टग्रेज या एसिंक्रोनस से लापता डेटा
प्रसंस्करण - [अधिक पढ़ें] (../ घटना- triggers.md)।

### व्युत्पन्न डेटा या डेटा परिवर्तन

ग्राफ़िकल इंजन का उपयोग करके अनुरोध किए जाने वाले डेटा का एक और सेट प्राप्त करने के लिए डेटा को पोस्टग्रेज या उस पर व्यावसायिक तर्क को चलाएं - [अधिक पढ़ें] (https://hasura.io/docs/1.0/graphql/manual/queries/derived-data .html)।

## डेमो

में उपलब्ध सभी उदाहरण देखें
[समुदाय / नमूना-ऐप्स] (.. / समुदाय / नमूना-ऐप्स) फ़ोल्डर।

### वास्तविक अनुप्रयोग

- एक ग्रुप मैसेजिंग एप्लिकेशन जो रिएक्ट का उपयोग करता है, उसमें टाइपिंग इंडिकेटर, ऑनलाइन उपयोगकर्ता और नए संदेशों की सूचनाएं शामिल हैं।
  - [अभी प्रयास करें] (https://realtime-chat.demo.hasura.app/)
  - [ट्यूटोरियल] (.. / समुदाय / नमूना-ऐप्स / रीयलटाइम-चैट)
  - (देखें एपीआई)] (https://realtime-chat.demo.hasura.app/console)

- वाहन के मानचित्र के आसपास चलते ही जीपीएस वाहन प्रदर्शित करता है कि लाइव वाहन स्थान ट्रैकिंग अनुप्रयोग।
  - [अभी प्रयास करें] (https://realtime-location-tracking.demo.hasura.app/)
  - [ट्यूटोरियल] (.. / समुदाय / नमूना-ऐप्स / रीयलटाइम-स्थान-ट्रैकिंग)
  - (देखें एपीआई) (https://realtime-location-tracking.demo.hasura.app/console)

- वास्तविक समय का डैशबोर्ड जो लगातार बदलते डेटा पर डेटा को एकीकृत करता है।
  - [अभी प्रयास करें] (https://realtime-poll.demo.hasura.app/)
  - [ट्यूटोरियल] (.. / समुदाय / नमूना-ऐप्स / रियलटाइम-पोल)
  - (देखें एपीआई)] (https://realtime-poll.demo.hasura.app/console)
  
  ## समर्थन और समस्या निवारण

दस्तावेज़ीकरण और समुदाय आपको कई समस्याओं को हल करने में मदद करेंगे। यदि आप बग ढूंढते हैं या हमसे संपर्क करना चाहते हैं, तो आप हमें नीचे दिए गए चैनलों पर पा सकते हैं:

* समर्थन और प्रतिक्रिया: [त्याग] (https://discord.gg/vBPpJkS)
* समस्या और बग ट्रैकिंग: [गिटहब मुद्दे] (https://github.com/hasura/graphql-engine/issive)
* उत्पाद अपडेट का पालन करें: [@HasuraHQ] (https://twitter.com/hasurahq)
* हमसे [हमारी वेबसाइट] (https://hasura.io) पर बात करें

हम समुदाय में एक खुले और स्वागत योग्य वातावरण का पोषण करने के लिए प्रतिबद्ध हैं। कृपया [आचार संहिता] (../ कोड-of-conduct.md) देखें।

यदि आप सुरक्षा भेद्यता की रिपोर्ट करना चाहते हैं, तो कृपया [इसे पढ़ें] (../ SECURITY.md)।

## योगदान

अधिक जानकारी के लिए हमारा [योगदान गाइड] (../ CONTRIBUTING.md) देखें।

## ब्रांडेड सामग्री

हसुरा ब्रांडेड सामग्री (लोगो, हसुरा शुभंकर, बैज आदि द्वारा संचालित) [परिसंपत्तियों / ब्रांड] (../ आस्तियों / ब्रांड) फ़ोल्डर में पाई जा सकती है। अपने आवेदन / वेबसाइट में उनका उपयोग करने के लिए स्वतंत्र महसूस करें। अगर आपने हसुरा की मदद से अपने एप्लिकेशन में "लॉन्च हसुरा" बैज जोड़ दिया तो हमें भी खुशी होगी। ❤️

<div style = "display: flex;">
  <img src = "../ आस्तियाँ / ब्रांड / संचालित_by_hasura_blue.svg" चौड़ाई = "150px" />
  <img src = "../ एसेट्स / ब्रांड / संचालित_बीज_हसुरा_व्हाईट" svg "चौड़ाई =" 150px "/>
</ Div>

`` `html
<! - उज्ज्वल पृष्ठभूमि के लिए ->
<a href="https://hasura.io">
  <img चौड़ाई = "150px" src = "https://graphql-engine-cdn.hasura.io/img/powered_by_hasura_blue.svg" />
</a>

<! - डार्क बैकग्राउंड के लिए ->
<a href="https://hasura.io">
  <img चौड़ाई = "150px" src = "https://graphql-engine-cdn.hasura.io/img/powered_by_hasura_white.svg" />
</a>
`` `
## लाइसेंस

GraphQL इंजन [Apache लाइसेंस 2.0] (https://www.apache.org/licenses/LICENSE-2.0) (Apache-2.0) के तहत उपलब्ध है।

सभी ** अन्य सामग्री ** (सिवाय इसके कि [`सर्वर`] में) (.. / सर्वर), [` cli`] (../ cli) और
[`कंसोल`] (.. / कंसोल) फ़ोल्डर] [एमआईटी लाइसेंस] (../ LICENSE- समुदाय) के तहत उपलब्ध हैं।
इसमें [`डॉक्स`] (../ डॉक्स) और [` समुदाय`] (../ समुदाय) सब कुछ शामिल है
नक्शे।

## अनुवाद

यह पृष्ठ निम्नलिखित भाषाओं में उपलब्ध है:

- [जापानी: jp:] (.. / अनुवाद / README.j जींस.md) (: प्रार्थना: [@ मोकसाहेरो] (https://github.com/moksahero))
- [फ्रेंच: fr:] (.. / अनुवाद / README.french.md) (: प्रार्थना: [@ l0ck3] (https://github.com/l0ck3))
- (एक ग्रीक [] (.. / अनुवाद / README.greek.md) (: प्रार्थना: [@ MIP2000] (https://github.com/MIP2000))
- [अंग्रेजी: uk:] (.. / अनुवाद / README.md)

अन्य फ़ाइलों के लिए अनुवाद [यहाँ] (.. / अनुवाद) पाया जा सकता है।