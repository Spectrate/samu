/**********************
Made by Nagy Áron
**********************/


1. Bontsd ki a linkgrammar tar.gz-t
2. cd linkgrammar-5.2.5
3. ./configure
4. make
5. sudo make install
6. sudo ldconfig

7. sudo ln -sv "$(pwd)/link-grammar/.libs/liblink-grammar.so.5" /usr/lib/
8. sudo ln -sv "$(pwd)/bindings/java-jni/.libs/liblink-grammar-java.so" /usr/lib/
Ha már létezne a liblink-grammar.so.5 és a liblink-grammar-java.so akkor nyugodtan töröld ki őket, és aztán add ki megint a parancsot.
(/usr/lib/ találod)


9.  Majd csomagold ki a java.tar.gz filet
10. Lépj be a kicsomagolt mappába
11. javac -cp /home/<felhasználónév>/Downloads/link-grammar-5.2.5/bindings/java/linkgrammar-5.2.5.jar *.java 
<felhasználónév> helyére írd a sajátod (feltéve, hogy a Downloads-ba töltötted le)
12. java -cp /home/robert/Downloads/link-grammar-5.2.5/bindings/java/linkgrammar-5.2.5.jar:`pwd` Main
úgyszintén a linkgrammar utvonala

