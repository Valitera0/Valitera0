 Def fonction _Et (a,b) : 

 Return a and b 

#calcul du tableau de verité 

Def table_verité() : 

 Valeurs =[fals ,true] 

 Print(« table de verité pour la fonction loogique Et : ») 

 Print(……………………………………………………………………….) 

 For a,b in product(valeurs,repeat=2) : 

 Resultat=int(fonction_Et (a,b)) 

 Print (f »{int(a)} {int(b)} {Resultat} ») 

#calcul de la premiere forme canonique 

 Def premiere_forme_canonique() : 

 Print ( « \n premiere forme canonique pour la fonctionlogique Et : ») 

 Print ( « F= A.B +A’ .B+A.B’+A’ .B’ »)# En utilisant la notation F pour le resulttat , 

 A et B pour les entrées , et A’ et B ‘pour les négations 

# calcul de la deuxième forme canonique 

Def deuxième _ forme _ canonique() : 

 Print(« \n deuxième forme canonique pour la fonction logique Et : ») 
 Print ( « F=¬m(0, 3) »representation sous forme de mintermes (produit des termes qui produisent 

un resultat vrai pour la fonction logique 

#Appel des fonctions pour afficher le tableau de verité et les formes canonique 

Table_verité() 

Premiere_forme_canonique 

Deuxieme_forme_canonique 

Exercice 2 : Ecrivons un algoritheme et programme en Python permettant de minimiser une fonction 

logique donné par la methode de KARNAUGH. 

1-Definir la fonction logique donnée sous forme de tableau de verité ou en utilisant les terme 

canoniques 

2- construire une carte de Karnaugh à partir des valeur de fonction logique et identifier les 

regroupements possibles de cellules contenant des « 1 » dans la carte . 

3-Identifier les termes dans le groupements spécifiés par la carte de Karnaugh , 

#Definition de la fonction logique « or »a trois entrées sous forme de tableau de verité 

Table_de _verité={(false,false,false) :false, 

 (false,false,true) :true, 

 (false,true ,false) :false , 

 (false,true,true) :true, 

 (true,false,false) :false , 

 (true,false,true) :true, 

 (true,true,false) :true, 

 (true,true,true) :true ,} 

#construction de la carte de Karnaugh pour la fonction logique « or » àtrois entrées 

Def Karnaugh_map() : 

 Print (« Karaugh Map for the or function with 3 inputs : ») 

 Print(« ABC/00/01/11/10 « ) 

 Print («……………………………….) 
 For a,b,c in product ([false,true], repeat= 3° : 

 Resultat=int (table_de_verité[ (a,b,c)] ) 

 Print ( f » { int(a) }{int(b) } {int(c)} / {int (table_de_verité[ (a,b,c)] ) } « ) 

#minimisation de la fonction lopgique à l`aide de la carte de Karnaugh 

Def minimisation_Karnaugh() : 

 Termes_essentiels =[]# liste por stocker les termes essentiels 

 Termas_non_essentiels=[]#liste pour stocker les termes non essentiels 

 For combinaison,valeur in table_de_verité,items() : 

 If valeur :# chercher les « 1 » dans le tableau de verité 

 Termes_essentiels .append(combinaison) ; 

 Print(« \n termes essentiels : »,termes_essentiels) 

#Trouver les termesnon essentiels 

For combinaison in table_de _verité_Keys() : 

 If combinaison not in termes_eszsentiels : 

 Termes _non_essentiels .append(combinaison) 

If le n (termes_non_essentiels) >0 : 

 Print( « termes non essentiels : »,termes_non_essentiels) 

 Print(« \n la fonction logique peut être simplifiée en regroupant les termes essentiels.°) 

#Appel des fonctions pour la construction de carte de Karnaugh et la minimisation de la fonction 

logique . 

Karnaugh_map() 

Minimisation_ Karnaugh() 
