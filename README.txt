###########################################################################################

	
	Les auteurs de ce projet sont:

		SOILIHI Mouchtali
		JANATI Mohammed

     Tous les deux en Masser 2 S�curit� des syst�mes information � universit� de Lorraine � Metz (2013/2014)


Un petit post sur un outil bien pratique pour tous ceux qui rament pour �crire des scripts sous Windows.
Un des outils indispensables dont toute production doive se doter est un analyseur de journaux d�erreur.

Logparser est un petit ex�cutable fourni gratuitement par Microsoft et qui permet de lire des fichiers structur�s
propri�taires tels que les eventlogs *.EVT, mais aussi les fichiers CVS, ETW, REG, etc� 
Tout d�abord il s�agit de le t�l�charger et de l�installer en trois ou quatre clics.
Je passe rapidement sur l�install, il faudra juste bien penser � ajouter le chemin de logparser.exe dans votre PATH.

Pour le t�l�charger:

http://www.microsoft.com/en-us/download/details.aspx?id=24659

L�avantage principal est qu�il utilise un pseudo langage proche du SQL pour effectuer des recherches. 


-i: Donne le type d�entr�e du fichier. exemple, -i:EVT indique que l�on souhaite lire un fichier *.evt. 
	S�il n�est pas indiqu�, logparser le trouve tout seul en fonction de l�entr�e.
-o: Donne le format de sortie. Par exemple -o:XML pour �crire au format XML.
	S�il n�est pas indiqu�, logparser le trouve tout seul en fonction du fichier indiqu� dans la clause �into�.
-stats: ON/OFF: si les stats sont indiqu�es, alors logparser renvoie le nombre de lignes trait�es et le temps pass�.
-q: ON/OFF: mode quiet, par exemple pour �liminer les ent�tes.
 INTO: Ceci permet d'enregister les resultats de la requete sur un fichier.
	 Into doit �tre plac� avant le FROM et il faut indiquer le chemin du fichier.


############################################################################################



