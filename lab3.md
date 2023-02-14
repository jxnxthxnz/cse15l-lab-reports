**The grep Command**

**-i Option**\
**Example 1**
```
find written_2/ > find-results.txt
grep -i "todo" find-results.txt
```
```
written_2//travel_guides/berlitz2/Amsterdam-WhatToDo.txt
written_2//travel_guides/berlitz2/CostaBlanca-WhatToDo.txt
written_2//travel_guides/berlitz2/Poland-WhatToDo.txt
written_2//travel_guides/berlitz2/Cuba-WhatToDo.txt
written_2//travel_guides/berlitz2/Cancun-WhatToDo.txt
written_2//travel_guides/berlitz2/Berlin-WhatToDo.txt
written_2//travel_guides/berlitz2/Bermuda-WhatToDo.txt
written_2//travel_guides/berlitz2/Budapest-WhatToDo.txt
written_2//travel_guides/berlitz2/PuertoRico-WhatToDo.txt
written_2//travel_guides/berlitz2/Vallarta-WhatToDo.txt
written_2//travel_guides/berlitz2/Bali-WhatToDo.txt
written_2//travel_guides/berlitz2/Portugal-WhatToDo.txt
written_2//travel_guides/berlitz2/Bahamas-WhatToDo.txt
written_2//travel_guides/berlitz2/Barcelona-WhatToDo.txt
written_2//travel_guides/berlitz2/Algarve-WhatToDo.txt
written_2//travel_guides/berlitz2/Costa-WhatToDo.txt
written_2//travel_guides/berlitz2/Crete-WhatToDo.txt
written_2//travel_guides/berlitz2/CanaryIslands-WhatToDo.txt
written_2//travel_guides/berlitz2/California-WhatToDo.txt
written_2//travel_guides/berlitz2/China-WhatToDo.txt
written_2//travel_guides/berlitz2/Athens-WhatToDo.txt
written_2//travel_guides/berlitz2/Nepal-WhatToDo.txt
written_2//travel_guides/berlitz2/Paris-WhatToDo.txt
written_2//travel_guides/berlitz2/Beijing-WhatToDo.txt
```
The -i option was used which means we can search for a specific string ("todo" in this example) insensitively (upper case and lower case does not make a difference). This option is useful when we want to search for a specifc word when there's both upper case and lower case versions of the word.\
Source: [Link](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

**Example 2**
```
find written_2/ > find-results.txt
grep -i "togo" find-results.txt
```
```
written_2//travel_guides/berlitz2/Berlin-WhereToGo.txt
written_2//travel_guides/berlitz2/Amsterdam-WhereToGo.txt
written_2//travel_guides/berlitz2/Costa-WhereToGo.txt
written_2//travel_guides/berlitz2/Portugal-WhereToGo.txt
written_2//travel_guides/berlitz2/Boston-WhereToGo.txt
written_2//travel_guides/berlitz2/California-WhereToGo.txt
written_2//travel_guides/berlitz2/Bahamas-WhereToGo.txt
written_2//travel_guides/berlitz2/Crete-WhereToGo.txt
written_2//travel_guides/berlitz2/Canada-WhereToGo.txt
written_2//travel_guides/berlitz2/Bali-WhereToGo.txt
written_2//travel_guides/berlitz2/Barcelona-WhereToGo.txt
written_2//travel_guides/berlitz2/Athens-WhereToGo.txt
written_2//travel_guides/berlitz2/Paris-WhereToGo.txt
written_2//travel_guides/berlitz2/China-WhereToGo.txt
written_2//travel_guides/berlitz2/CstaBlanca-WhereToGo.txt
written_2//travel_guides/berlitz2/PuertoRico-WhereToGo.txt
written_2//travel_guides/berlitz2/Cuba-WhereToGo.txt
written_2//travel_guides/berlitz2/Nepal-WhereToGo.txt
written_2//travel_guides/berlitz2/CanaryIslands-WhereToGo.txt
written_2//travel_guides/berlitz2/Algarve-WhereToGo.txt
written_2//travel_guides/berlitz2/Beijing-WhereToGo.txt
written_2//travel_guides/berlitz2/Bermuda-WhereToGo.txt
written_2//travel_guides/berlitz2/Vallarta-WhereToGo.txt
```
The -i option was used which means we can search for a specific string ("togo" in this example) insensitively (upper case and lower case does not make a difference). This option is useful when we want to search for a specifc word when there's both upper case and lower case versions of the word.\
Source: [Link](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

**-c Option**\
**Example 3**
```
find written_2/ > find-results.txt
grep -c "ToDo" find-results.txt
```
```
24
```
The -c option was used and allows us to count the number of lines that have a specific string ("ToDo" in this example). This option is useful when you have lots of lines and instead of manually counting which lines have a specific string, you can just use this command.\
Source: [Link](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

**Example 4**
```
find written_2/ > find-results.txt
grep -c "Fletcher" find-results.txt
```
```
7
```
The -c option was used and allows us to count the number of lines that have a specific string ("Fletcher" in this example). This option is useful when you have lots of lines and instead of manually counting which lines have a specific string, you can just use this command.\
Source: [Link](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

**-n Option**\
**Example 5**
```
find written_2/ > find-results.txt
grep -n "ToDo" find-results.txt
```
```
164:written_2//travel_guides/berlitz2/Amsterdam-WhatToDo.txt
165:written_2//travel_guides/berlitz2/CostaBlanca-WhatToDo.txt
169:written_2//travel_guides/berlitz2/Poland-WhatToDo.txt
171:written_2//travel_guides/berlitz2/Cuba-WhatToDo.txt
174:written_2//travel_guides/berlitz2/Cancun-WhatToDo.txt
178:written_2//travel_guides/berlitz2/Berlin-WhatToDo.txt
186:written_2//travel_guides/berlitz2/Bermuda-WhatToDo.txt
189:written_2//travel_guides/berlitz2/Budapest-WhatToDo.txt
191:written_2//travel_guides/berlitz2/PuertoRico-WhatToDo.txt
192:written_2//travel_guides/berlitz2/Vallarta-WhatToDo.txt
193:written_2//travel_guides/berlitz2/Bali-WhatToDo.txt
203:written_2//travel_guides/berlitz2/Portugal-WhatToDo.txt
206:written_2//travel_guides/berlitz2/Bahamas-WhatToDo.txt
207:written_2//travel_guides/berlitz2/Barcelona-WhatToDo.txt
208:written_2//travel_guides/berlitz2/Algarve-WhatToDo.txt
211:written_2//travel_guides/berlitz2/Costa-WhatToDo.txt
218:written_2//travel_guides/berlitz2/Crete-WhatToDo.txt
224:written_2//travel_guides/berlitz2/CanaryIslands-WhatToDo.txt
225:written_2//travel_guides/berlitz2/California-WhatToDo.txt
227:written_2//travel_guides/berlitz2/China-WhatToDo.txt
228:written_2//travel_guides/berlitz2/Athens-WhatToDo.txt
229:written_2//travel_guides/berlitz2/Nepal-WhatToDo.txt
231:written_2//travel_guides/berlitz2/Paris-WhatToDo.txt
235:written_2//travel_guides/berlitz2/Beijing-WhatToDo.txt
```
The -n option was used and allows us to find the lines that have a specific string ("ToDo" in this example) as well as the line number. This option is useful when you have lots of lines, and you can use the line number to find the specific line in the number rather than manually searching through it.\
Source: [Link](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

**Example 6**
```
find written_2/ > find-results.txt
grep -n "ToGo" find-results.txt
```
```
160:written_2//travel_guides/berlitz2/Berlin-WhereToGo.txt
162:written_2//travel_guides/berlitz2/Amsterdam-WhereToGo.txt
163:written_2//travel_guides/berlitz2/Costa-WhereToGo.txt
167:written_2//travel_guides/berlitz2/Portugal-WhereToGo.txt
168:written_2//travel_guides/berlitz2/Boston-WhereToGo.txt
170:written_2//travel_guides/berlitz2/California-WhereToGo.txt
173:written_2//travel_guides/berlitz2/Bahamas-WhereToGo.txt
176:written_2//travel_guides/berlitz2/Crete-WhereToGo.txt
179:written_2//travel_guides/berlitz2/Canada-WhereToGo.txt
180:written_2//travel_guides/berlitz2/Bali-WhereToGo.txt
182:written_2//travel_guides/berlitz2/Barcelona-WhereToGo.txt
183:written_2//travel_guides/berlitz2/Athens-WhereToGo.txt
184:written_2//travel_guides/berlitz2/Paris-WhereToGo.txt
185:written_2//travel_guides/berlitz2/China-WhereToGo.txt
195:written_2//travel_guides/berlitz2/CstaBlanca-WhereToGo.txt
209:written_2//travel_guides/berlitz2/PuertoRico-WhereToGo.txt
210:written_2//travel_guides/berlitz2/Cuba-WhereToGo.txt
213:written_2//travel_guides/berlitz2/Nepal-WhereToGo.txt
214:written_2//travel_guides/berlitz2/CanaryIslands-WhereToGo.txt
219:written_2//travel_guides/berlitz2/Algarve-WhereToGo.txt
223:written_2//travel_guides/berlitz2/Beijing-WhereToGo.txt
230:written_2//travel_guides/berlitz2/Bermuda-WhereToGo.txt
233:written_2//travel_guides/berlitz2/Vallarta-WhereToGo.txt
236:written_2//travel_guides/berlitz2/Cancun-WhereToGo.txt
```
The -n option was used and allows us to find the lines that have a specific string ("ToGo" in this example) as well as the line number. This option is useful when you have lots of lines, and you can use the line number to find the specific line in the number rather than manually searching through it.\
Source: [Link](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

**-v Option**\
**Example 7**
```
find written_2/ > find-results.txt
grep -v "-" find-results.txt
```
```
written_2/
written_2//travel_guides
written_2//travel_guides/berlitz1
written_2//travel_guides/berlitz1/HandRLasVegas.txt
written_2//travel_guides/berlitz1/HistoryJapan.txt
written_2//travel_guides/berlitz1/IntroMalaysia.txt
written_2//travel_guides/berlitz1/HandRIstanbul.txt
written_2//travel_guides/berlitz1/HistoryJamaica.txt
written_2//travel_guides/berlitz1/HandRJamaica.txt
written_2//travel_guides/berlitz1/HandRHongKong.txt
written_2//travel_guides/berlitz1/HistoryEgypt.txt
written_2//travel_guides/berlitz1/IntroEdinburgh.txt
written_2//travel_guides/berlitz1/HistoryIsrael.txt
written_2//travel_guides/berlitz1/IntroDublin.txt
written_2//travel_guides/berlitz1/HistoryIndia.txt
written_2//travel_guides/berlitz1/IntroFrance.txt
written_2//travel_guides/berlitz1/IntroMadeira.txt
written_2//travel_guides/berlitz1/WhatToLakeDistrict.txt
written_2//travel_guides/berlitz1/IntroIbiza.txt
written_2//travel_guides/berlitz1/HistoryItaly.txt
written_2//travel_guides/berlitz1/WhereToGreek.txt
written_2//travel_guides/berlitz1/WhereToLakeDistrict.txt
written_2//travel_guides/berlitz1/HistoryDublin.txt
written_2//travel_guides/berlitz1/IntroIsrael.txt
written_2//travel_guides/berlitz1/WhatToIbiza.txt
written_2//travel_guides/berlitz1/HistoryFrance.txt
written_2//travel_guides/berlitz1/WhatToHawaii.txt
written_2//travel_guides/berlitz1/HistoryMallorca.txt
written_2//travel_guides/berlitz1/HistoryJerusalem.txt
written_2//travel_guides/berlitz1/HandRLisbon.txt
written_2//travel_guides/berlitz1/WhereToIndia.txt
written_2//travel_guides/berlitz1/HistoryMadrid.txt
written_2//travel_guides/berlitz1/HistoryHongKong.txt
written_2//travel_guides/berlitz1/IntroMadrid.txt
written_2//travel_guides/berlitz1/IntroLosAngeles.txt
written_2//travel_guides/berlitz1/HistoryIstanbul.txt
written_2//travel_guides/berlitz1/WhereToItaly.txt
written_2//travel_guides/berlitz1/HistoryLasVegas.txt
written_2//travel_guides/berlitz1/HistoryGreek.txt
written_2//travel_guides/berlitz1/HandRMallorca.txt
written_2//travel_guides/berlitz1/JungleMalaysia.txt
written_2//travel_guides/berlitz1/WhatToMadeira.txt
written_2//travel_guides/berlitz1/WhatToFWI.txt
written_2//travel_guides/berlitz1/WhereToMalaysia.txt
written_2//travel_guides/berlitz1/WhatToMalaysia.txt
written_2//travel_guides/berlitz1/WhatToDublin.txt
written_2//travel_guides/berlitz1/WhereToJapan.txt
written_2//travel_guides/berlitz1/HistoryHawaii.txt
written_2//travel_guides/berlitz1/WhatToFrance.txt
written_2//travel_guides/berlitz1/WhereToEgypt.txt
written_2//travel_guides/berlitz1/WhereToEdinburgh.txt
written_2//travel_guides/berlitz1/WhatToIsrael.txt
written_2//travel_guides/berlitz1/HandRLosAngeles.txt
written_2//travel_guides/berlitz1/HistoryMadeira.txt
written_2//travel_guides/berlitz1/IntroJerusalem.txt
written_2//travel_guides/berlitz1/HandRMadeira.txt
written_2//travel_guides/berlitz1/WhereToIsrael.txt
written_2//travel_guides/berlitz1/HandRIbiza.txt
written_2//travel_guides/berlitz1/WhereToFrance.txt
written_2//travel_guides/berlitz1/WhereToDublin.txt
written_2//travel_guides/berlitz1/IntroLasVegas.txt
written_2//travel_guides/berlitz1/IntroIstanbul.txt
written_2//travel_guides/berlitz1/WhereToMallorca.txt
written_2//travel_guides/berlitz1/WhatToMallorca.txt
written_2//travel_guides/berlitz1/IntroHongKong.txt
written_2//travel_guides/berlitz1/IntroFWI.txt
written_2//travel_guides/berlitz1/IntroJamaica.txt
written_2//travel_guides/berlitz1/IntroGreek.txt
written_2//travel_guides/berlitz1/HandRIsrael.txt
written_2//travel_guides/berlitz1/WhatToEdinburgh.txt
written_2//travel_guides/berlitz1/WhereToMadeira.txt
written_2//travel_guides/berlitz1/WhatToGreek.txt
written_2//travel_guides/berlitz1/HandRLakeDistrict.txt
written_2//travel_guides/berlitz1/WhereToIbiza.txt
written_2//travel_guides/berlitz1/WhereToHawaii.txt
written_2//travel_guides/berlitz1/HandRMadrid.txt
written_2//travel_guides/berlitz1/HistoryMalaysia.txt
written_2//travel_guides/berlitz1/IntroItaly.txt
written_2//travel_guides/berlitz1/WhatToIndia.txt
written_2//travel_guides/berlitz1/WhereToLosAngeles.txt
written_2//travel_guides/berlitz1/HandRJerusalem.txt
written_2//travel_guides/berlitz1/HistoryIbiza.txt
written_2//travel_guides/berlitz1/HistoryEdinburgh.txt
written_2//travel_guides/berlitz1/HistoryFWI.txt
written_2//travel_guides/berlitz1/IntroIndia.txt
written_2//travel_guides/berlitz1/WhatToItaly.txt
written_2//travel_guides/berlitz1/HistoryLakeDistrict.txt
written_2//travel_guides/berlitz1/WhereToMadrid.txt
written_2//travel_guides/berlitz1/WhereToJerusalem.txt
written_2//travel_guides/berlitz1/IntroEgypt.txt
written_2//travel_guides/berlitz1/HandRHawaii.txt
written_2//travel_guides/berlitz1/WhatToJapan.txt
written_2//travel_guides/berlitz1/WhatToJamaica.txt
written_2//travel_guides/berlitz1/IntroLakeDistrict.txt
written_2//travel_guides/berlitz1/IntroMallorca.txt
written_2//travel_guides/berlitz1/WhatToHongKong.txt
written_2//travel_guides/berlitz1/WhatToEgypt.txt
written_2//travel_guides/berlitz1/WhereToHongKong.txt
written_2//travel_guides/berlitz1/WhereToFWI.txt
written_2//travel_guides/berlitz1/WhatToIstanbul.txt
written_2//travel_guides/berlitz1/WhereToIstanbul.txt
written_2//travel_guides/berlitz1/IntroJapan.txt
written_2//travel_guides/berlitz1/WhatToLasVegas.txt
written_2//travel_guides/berlitz1/WhatToLosAngeles.txt
written_2//travel_guides/berlitz2
```
The -v option was used and allows us to find the lines that don't have a specific string ("-" in this example). This option is useful when you want to filter through a file based on a specific string and see the lines that don't match rather than the ones that do.\
Source: [Link](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

**Example 8**
```
find written_2/ > find-results.txt
grep -v "To" find-results.txt
```
```
written_2/
written_2//non-fiction
written_2//non-fiction/OUP
written_2//non-fiction/OUP/Berk
written_2//non-fiction/OUP/Berk/ch2.txt
written_2//non-fiction/OUP/Berk/ch1.txt
written_2//non-fiction/OUP/Berk/CH4.txt
written_2//non-fiction/OUP/Berk/ch7.txt
written_2//non-fiction/OUP/Abernathy
written_2//non-fiction/OUP/Abernathy/ch2.txt
written_2//non-fiction/OUP/Abernathy/ch3.txt
written_2//non-fiction/OUP/Abernathy/ch1.txt
written_2//non-fiction/OUP/Abernathy/ch7.txt
written_2//non-fiction/OUP/Abernathy/ch6.txt
written_2//non-fiction/OUP/Abernathy/ch8.txt
written_2//non-fiction/OUP/Abernathy/ch9.txt
written_2//non-fiction/OUP/Abernathy/ch15.txt
written_2//non-fiction/OUP/Abernathy/ch14.txt
written_2//non-fiction/OUP/Rybczynski
written_2//non-fiction/OUP/Rybczynski/ch2.txt
written_2//non-fiction/OUP/Rybczynski/ch3.txt
written_2//non-fiction/OUP/Rybczynski/ch1.txt
written_2//non-fiction/OUP/Kauffman
written_2//non-fiction/OUP/Kauffman/ch3.txt
written_2//non-fiction/OUP/Kauffman/ch1.txt
written_2//non-fiction/OUP/Kauffman/ch4.txt
written_2//non-fiction/OUP/Kauffman/ch5.txt
written_2//non-fiction/OUP/Kauffman/ch7.txt
written_2//non-fiction/OUP/Kauffman/ch6.txt
written_2//non-fiction/OUP/Kauffman/ch8.txt
written_2//non-fiction/OUP/Kauffman/ch9.txt
written_2//non-fiction/OUP/Kauffman/ch10.txt
written_2//non-fiction/OUP/Fletcher
written_2//non-fiction/OUP/Fletcher/ch2.txt
written_2//non-fiction/OUP/Fletcher/ch1.txt
written_2//non-fiction/OUP/Fletcher/ch5.txt
written_2//non-fiction/OUP/Fletcher/ch6.txt
written_2//non-fiction/OUP/Fletcher/ch9.txt
written_2//non-fiction/OUP/Fletcher/ch10.txt
written_2//non-fiction/OUP/Castro
written_2//non-fiction/OUP/Castro/chR.txt
written_2//non-fiction/OUP/Castro/chP.txt
written_2//non-fiction/OUP/Castro/chQ.txt
written_2//non-fiction/OUP/Castro/chB.txt
written_2//non-fiction/OUP/Castro/chC.txt
written_2//non-fiction/OUP/Castro/chA.txt
written_2//non-fiction/OUP/Castro/chV.txt
written_2//non-fiction/OUP/Castro/chW.txt
written_2//non-fiction/OUP/Castro/chM.txt
written_2//non-fiction/OUP/Castro/chZ.txt
written_2//non-fiction/OUP/Castro/chL.txt
written_2//non-fiction/OUP/Castro/chN.txt
written_2//non-fiction/OUP/Castro/chY.txt
written_2//non-fiction/OUP/Castro/chO.txt
written_2//travel_guides
written_2//travel_guides/berlitz1
written_2//travel_guides/berlitz1/HandRLasVegas.txt
written_2//travel_guides/berlitz1/HistoryJapan.txt
written_2//travel_guides/berlitz1/IntroMalaysia.txt
written_2//travel_guides/berlitz1/HandRIstanbul.txt
written_2//travel_guides/berlitz1/HistoryJamaica.txt
written_2//travel_guides/berlitz1/HandRJamaica.txt
written_2//travel_guides/berlitz1/HandRHongKong.txt
written_2//travel_guides/berlitz1/HistoryEgypt.txt
written_2//travel_guides/berlitz1/IntroEdinburgh.txt
written_2//travel_guides/berlitz1/HistoryIsrael.txt
written_2//travel_guides/berlitz1/IntroDublin.txt
written_2//travel_guides/berlitz1/HistoryIndia.txt
written_2//travel_guides/berlitz1/IntroFrance.txt
written_2//travel_guides/berlitz1/IntroMadeira.txt
written_2//travel_guides/berlitz1/IntroIbiza.txt
written_2//travel_guides/berlitz1/HistoryItaly.txt
written_2//travel_guides/berlitz1/HistoryDublin.txt
written_2//travel_guides/berlitz1/IntroIsrael.txt
written_2//travel_guides/berlitz1/HistoryFrance.txt
written_2//travel_guides/berlitz1/HistoryMallorca.txt
written_2//travel_guides/berlitz1/HistoryJerusalem.txt
written_2//travel_guides/berlitz1/HandRLisbon.txt
written_2//travel_guides/berlitz1/HistoryMadrid.txt
written_2//travel_guides/berlitz1/HistoryHongKong.txt
written_2//travel_guides/berlitz1/IntroMadrid.txt
written_2//travel_guides/berlitz1/IntroLosAngeles.txt
written_2//travel_guides/berlitz1/HistoryIstanbul.txt
written_2//travel_guides/berlitz1/HistoryLasVegas.txt
written_2//travel_guides/berlitz1/HistoryGreek.txt
written_2//travel_guides/berlitz1/HandRMallorca.txt
written_2//travel_guides/berlitz1/JungleMalaysia.txt
written_2//travel_guides/berlitz1/HistoryHawaii.txt
written_2//travel_guides/berlitz1/HandRLosAngeles.txt
written_2//travel_guides/berlitz1/HistoryMadeira.txt
written_2//travel_guides/berlitz1/IntroJerusalem.txt
written_2//travel_guides/berlitz1/HandRMadeira.txt
written_2//travel_guides/berlitz1/HandRIbiza.txt
written_2//travel_guides/berlitz1/IntroLasVegas.txt
written_2//travel_guides/berlitz1/IntroIstanbul.txt
written_2//travel_guides/berlitz1/IntroHongKong.txt
written_2//travel_guides/berlitz1/IntroFWI.txt
written_2//travel_guides/berlitz1/IntroJamaica.txt
written_2//travel_guides/berlitz1/IntroGreek.txt
written_2//travel_guides/berlitz1/HandRIsrael.txt
written_2//travel_guides/berlitz1/HandRLakeDistrict.txt
written_2//travel_guides/berlitz1/HandRMadrid.txt
written_2//travel_guides/berlitz1/HistoryMalaysia.txt
written_2//travel_guides/berlitz1/IntroItaly.txt
written_2//travel_guides/berlitz1/HandRJerusalem.txt
written_2//travel_guides/berlitz1/HistoryIbiza.txt
written_2//travel_guides/berlitz1/HistoryEdinburgh.txt
written_2//travel_guides/berlitz1/HistoryFWI.txt
written_2//travel_guides/berlitz1/IntroIndia.txt
written_2//travel_guides/berlitz1/HistoryLakeDistrict.txt
written_2//travel_guides/berlitz1/IntroEgypt.txt
written_2//travel_guides/berlitz1/HandRHawaii.txt
written_2//travel_guides/berlitz1/IntroLakeDistrict.txt
written_2//travel_guides/berlitz1/IntroMallorca.txt
written_2//travel_guides/berlitz1/IntroJapan.txt
written_2//travel_guides/berlitz2
written_2//travel_guides/berlitz2/Portugal-History.txt
written_2//travel_guides/berlitz2/Costa-History.txt
written_2//travel_guides/berlitz2/Barcelona-History.txt
written_2//travel_guides/berlitz2/Berlin-History.txt
written_2//travel_guides/berlitz2/Bali-History.txt
written_2//travel_guides/berlitz2/Athens-History.txt
written_2//travel_guides/berlitz2/Budapest-WhereoGo.txt
written_2//travel_guides/berlitz2/California-History.txt
written_2//travel_guides/berlitz2/Vallarta-History.txt
written_2//travel_guides/berlitz2/Cancun-History.txt
written_2//travel_guides/berlitz2/CostaBlanca-History.txt
written_2//travel_guides/berlitz2/NewOrleans-History.txt
written_2//travel_guides/berlitz2/PuertoRico-History.txt
written_2//travel_guides/berlitz2/Algarve-Intro.txt
written_2//travel_guides/berlitz2/Nepal-History.txt
written_2//travel_guides/berlitz2/China-History.txt
written_2//travel_guides/berlitz2/Canada-History.txt
written_2//travel_guides/berlitz2/Crete-History.txt
written_2//travel_guides/berlitz2/Bahamas-Intro.txt
written_2//travel_guides/berlitz2/Amsterdam-History.txt
written_2//travel_guides/berlitz2/Beijing-History.txt
written_2//travel_guides/berlitz2/Bermuda-history.txt
written_2//travel_guides/berlitz2/CanaryIslands-History.txt
written_2//travel_guides/berlitz2/Amsterdam-Intro.txt
written_2//travel_guides/berlitz2/Athens-Intro.txt
written_2//travel_guides/berlitz2/Algarve-History.txt
written_2//travel_guides/berlitz2/Poland-History.txt
written_2//travel_guides/berlitz2/Budapest-History.txt
written_2//travel_guides/berlitz2/Cuba-History.txt
written_2//travel_guides/berlitz2/Bahamas-History.txt
```
The -v option was used and allows us to find the lines that don't have a specific string ("To" in this example). This option is useful when you want to filter through a file based on a specific string and see the lines that don't match rather than the ones that do.\
Source: [Link](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)
