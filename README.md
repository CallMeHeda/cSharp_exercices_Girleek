[![My Skills](https://skillicons.dev/icons?i=cs)](https://skillicons.dev)

using System;
using System.Collections.Generic;
					
public class Program
{
	# Exercice 6: Introduction aux Fonctions
    static void Afficher(int nb){
		Console.WriteLine("Le nombre est : " + nb);
	}
	
	# Exercice 7: Fonctions et Méthodes
	static int Somme(int nb1, int nb2){
		return nb1 + nb2;
	}
	
	# Exercice 8: Portée des Variables
	## Variable Globale
	static bool globale =  true;
	
	# Exercice 9: Programmation Orientée Objet
	class Animal{
		public string Nom;
	}
	
	# Exercice 10: Concepts Orientés Objet
	class Animal{
		public string Nom;
		public void FaireDuBruit(string noise){
			Console.WriteLine(noise);
		}
	}
	
	public static void Main()
	{
		# Exercice 1: Variables et Types de Données
		int nb = 42;
		string hello = "Hello world";
		double nbFloat = 42.42;
		
		Console.WriteLine("Entier : " + nb + " - Chaine de caractères : " + hello + " - Nombre décimal : " + nbFloat );
		
		# Exercice 1: Variables et Types de Données - Améliorée
		int nb;
		string hello;
		double nbFloat;
		
		Console.WriteLine("Entrez un entier :");
		string data = Console.ReadLine();
		nb = int.Parse(data);
		Console.WriteLine("Entrez une chaine de caractères :");
		hello = Console.ReadLine();
		Console.WriteLine("Entrez un nombre décimal :");
		string dataDouble = Console.ReadLine();
		nbFloat = double.Parse(dataDouble);
		
		Console.WriteLine("Entier : " + nb + " - Chaine de caractères : " + hello + " - Nombre décimal : " + nbFloat );
		
		# Exercice 2: Types de Données
		bool sunny = false;
		Console.WriteLine(sunny);
		
		# Exercice 3 : Opérations sur les Variables
		int nb1 = 42;
		int nb2 = 41;
		int somme = nb1 + nb2;
		Console.WriteLine(somme);
		
		# Exercice 4: Structures de Contrôle
		int nb;
		
		Console.WriteLine("Entrez un nombre :");
		string data = Console.ReadLine();
		nb = int.Parse(data);
		
		while(nb != 0){
			if(nb > 0){
				Console.WriteLine("Le nombre : " + nb + " est positif");
			}else{
				Console.WriteLine("Le nombre : " + nb + " est négatif");
			}
			
			Console.WriteLine("Entrez un nombre :");
            data = Console.ReadLine();
            nb = int.Parse(data);
		}
		
		# Exercice 5: Boucles
		for (int i = 1; i <= 5; i++){
			Console.WriteLine(i);
		}
		
		# Exercice 6: Introduction aux Fonctions
		Afficher(42);
		
		# Exercice 7: Fonctions et Méthodes
		Console.WriteLine(Somme(5,10));
		
		# Exercice 8: Portée des Variables
		## Variable Locale
		bool sunny = false;

		Console.WriteLine(globale);
		Console.WriteLine(sunny);
		
		# Exercice 9: Programmation Orientée Objet
		Animal lion = new Animal();
		lion.Nom = "Simba";
		Console.WriteLine(lion.Nom);
		
		# Exercice 10: Concepts Orientés Objet
		Animal cat = new Animal();
		cat.FaireDuBruit("Miaou");
		
		# Exercice 11: Gestion des Exceptions
		try{
			 Console.WriteLine("Entrez le premier nombre :");
             string data1 = Console.ReadLine();
             double nb1 = double.Parse(data1);

             Console.WriteLine("Entrez le deuxième nombre :");
             string data2 = Console.ReadLine();
             double nb2 = double.Parse(data2);
			 
			 if (nb2 == 0){
				 Console.WriteLine("Erreur : Division par zéro.");
			 }else{
				 double result = nb1 / nb2;
				 Console.WriteLine("Le résultat : " + result);
			 }
		 }catch (Exception e){
			 Console.WriteLine(e);
		 }
		
		# Exercice 12: Collections et Génériques
		List<int> listOfNumbers = new List<int>();
		listOfNumbers.AddRange(new int[] { 2, 40, 8, 42, 105 }); // Add pour ajouter un seul nombre et AddRange pour en ajouter plusieurs à la fois
		
		foreach (int number in listOfNumbers){
			Console.WriteLine(number);
		}
	}
}
