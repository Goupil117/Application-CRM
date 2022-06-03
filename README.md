# Application CRM Lourde

<h3>Sommaire :</h3>
<li><a href="#presentation">Présentation de l'application</a></li>
<li><a href="#docs">Documentation développeur</a></li>
<li><a href="#credits">Crédits</a></li>

<h2 id="presentation">Présentation de l'application</h2>

<p>L'application CRM Lourde est une application de type Windows développer en C# avec le framework WPF, permettant l’ajout, la modification<br>
et la Suppression des clients, des prospects, des rendez-vous et la visualisation des factures.</p>

<p>Interface principale :</p>

<img src="img\App.png"/>

<p>Onglets</p>

<img src="img\Menus.png"/>

<p>Zone d'affichage des différentes données</p>

<img src="img\Datas.png"/>

<p>Interface pour modifier, ajouter, ou supprimer des données</p>

<img src="img\Form.png"/>

<p>Zone de paramètres pour changer la base de données utilisée</p>

<img src="img\Settings.png"/>

<h2 id="docs">Documentation développeur</h2>

<p>L'application a été développée en langage C# utilisant le framework WPF<br>
à l'aide du logiciel Visual Studio 2019 développé par Microsoft.</p>

<h3>Classe présente dans l'application</h3>

<ul>
    <li>Client</li>
    <li>Commercial</li>
    <li>Prospect</li>
    <li>Produit</li>
    <li>Facture</li>
    <li>Rendez-vous</li>
    <li>Contact</li>
    <li>MySql_Database</li>
</ul>

</br>

<h4>Contructeur de la classe Client :</h4>

```
	public Client()
        {

        }

		public Client(int id)
        {
			Id = id;
        }

		public Client(string nom, string prenom, string telephone, string email, string adresse, string ville, string code_postal)
        {
            Nom = nom;
            Prenom = prenom;
            Telephone = telephone;
            Email = email;
            Adresse = adresse;
            Ville = ville;
            Code_Postal = code_postal;
        }

        public Client(int id, string nom, string prenom, string telephone, string email, string adresse, string ville, string code_postal)
        {
            Id = id;
            Nom = nom;
            Prenom = prenom;
            Telephone = telephone;
            Email = email;
            Adresse = adresse;
            Ville = ville;
            Code_Postal = code_postal;
        }
```

<h4>Contructeur de la classe Commercial :</h4>
```
        public Commercial()
        {

        }

        public Commercial(int id)
        {
            Id = id;
        }

        public Commercial(string nom, string prenom, string telephone, string email)
        {
            Nom = nom;
            Prenom = prenom;
            Telephone = telephone;
            Email = email;
        }

        public Commercial(int id, string nom, string prenom, string telephone, string email)
        {
            Id = id;
            Nom = nom;
            Prenom = prenom;
            Telephone = telephone;
            Email = email;
        }
```

<h4>Contructeur de la classe Commercial :</h4>
```
        public Contact()
        {

        }

        public Contact(int id)
        {
            Id = id;
        }

        public Contact(string nom, string prenom, string telephone, string email, string adresse, string ville, string code_postal)
        {
            Nom = nom;
            Prenom = prenom;
            Telephone = telephone;
            Email = email;
            Adresse = adresse;
            Ville = ville;
            Code_Postal = code_postal;
        }

        public Contact(int id, string nom, string prenom, string telephone, string email, string adresse, string ville, string code_postal)
        {
            Id = id;
            Nom = nom;
            Prenom = prenom;
            Telephone = telephone;
            Email = email;
            Adresse = adresse;
            Ville = ville;
            Code_Postal = code_postal;
        }
```

<h4>Contructeur de la classe Prospects :</h4>
```
        public Prospect()
        {

        }

        public Prospect(int id)
        {
            Id = id;
        }

        public Prospect(string nom, string prenom)
        {
            Nom = nom;
            Prenom = prenom;
        }

        public Prospect(string nom, string prenom, string telephone, string email, string adresse, string ville, string code_postal)
        {
            Nom = nom;
            Prenom = prenom;
            Telephone = telephone;
            Email = email;
            Adresse = adresse;
            Ville = ville;
            Code_Postal = code_postal;
        }

        public Prospect(int id, string nom, string prenom, string telephone, string email, string adresse, string ville, string code_postal)
        {
            Id = id;
            Nom = nom;
            Prenom = prenom;
            Telephone = telephone;
            Email = email;
            Adresse = adresse;
            Ville = ville;
            Code_Postal = code_postal;
        }
```

<h4>Contructeur de la classe Produit :</h4>
```
	public Produit()
        {

        }

        public Produit(string nom, string description, double prix)
        {
            Nom = nom;
            Prix = prix;
            Description = description;
        }

        public Produit(int id, string nom, string description, double prix)
        {
            Id = id;
            Nom = nom;
            Prix = prix;
            Description = description;
        }
```

<h4>Contructeur de la classe Facture :</h4>
```
	public Facture()
        {

        }

        public Facture(int id)
        {
            Id = id;
        }

        public Facture(int id, Client client, Produit produit, int quantite, DateTime date, double montant)
        {
            Id = id;
            Client = client;
            Produit = produit;
            Quantite = quantite;
            Date = date;
            Montant = montant;
        }

        public Facture(Client client, Produit produit, int quantite, DateTime date, double montant)
        {
            Client = client;
            Produit = produit;
            Quantite = quantite;
            Date = date;
            Montant = montant;
        }
```

<h4>Contructeur de la classe Rendez-vous :</h4>
```
 	public Rendez_Vous()
        {

        }
        public Rendez_Vous(int id, DateTime date, Commercial commercial, Contact contact, string lieux)
        {
            Id = id;
            Date = date;
            Commercial = commercial;
            Contact = contact;
            Lieux = lieux;
        }

        public Rendez_Vous(DateTime date, Commercial commercial, Contact contact, string lieux)
        {
            Date = date;
            Commercial = commercial;
            Contact = contact;
            Lieux = lieux;
        }
```

<h4>Contructeur de la classe Contact :</h4>
```
        public Contact()
        {

        }

        public Contact(int id)
        {
            Id = id;
        }

        public Contact(string nom, string prenom, string telephone, string email, string adresse, string ville, string code_postal)
        {
            Nom = nom;
            Prenom = prenom;
            Telephone = telephone;
            Email = email;
            Adresse = adresse;
            Ville = ville;
            Code_Postal = code_postal;
        }

        public Contact(int id, string nom, string prenom, string telephone, string email, string adresse, string ville, string code_postal)
        {
            Id = id;
            Nom = nom;
            Prenom = prenom;
            Telephone = telephone;
            Email = email;
            Adresse = adresse;
            Ville = ville;
            Code_Postal = code_postal;
        }
```

<h4>Contructeur de la classe MySql_Database :</h4>
```
	public MySql_Database()
        {
            Connexion_BD();
        }

        public MySql_Database(string Serveur, string User, string Password, string DataBase)
        {
            serveur = Serveur;
            user = User;
            password = Password;
            database = DataBase;

            Connexion_BD();
        }
```


<p>Elle récupère les informations de la base de données utilisant cette méthode</p>

```
        public List<List> GetList()
        {
            try
            {
                requete = "select * from table";

                connexion.Open();

                MySqlCommand commande = new MySqlCommand(requete, connexion);
                MySqlDataReader resultat = commande.ExecuteReader();

                List<List> cList = new List<List>();

                while (resultat.Read())
                {
                    List tmpList = new List(
                        Convert.ToInt32(resultat["Number"]), 
                        Convert.ToString(resultat["String"]));
                    cList.Add(tmpList);
                }

                connexion.Close();
                return cList;
            }
            catch (MySqlException error)
            {
                connexion.Close();
                Console.WriteLine("Erreur GetList : " + error.Message);
                return new List<List>();
            }

        }
```

<p>Elle ajoute des données dans la base de données utilisant cette méthode</p>

```
        public void PostList(List List)
        {
            try
            {
                requete = "INSERT INTO table(number, text) VALUES (@Number, @Text)";

                connexion.Open();

                MySqlCommand commande = new MySqlCommand(requete, connexion);

                commande.Parameters.AddWithValue("@Number", List.NUMBER);
                commande.Parameters.AddWithValue("@Text", List.TEXT);

                commande.ExecuteNonQuery();

                connexion.Close();
            }
            catch (MySqlException ex)
            {
                connexion.Close();
                Console.WriteLine("Erreur PostList : " + ex.Message);
            }
        }
```

<p>Elle modifie des données dans la base de données utilisant cette méthode</p>

```
        public void PutList(List List)
        {
            try
            {
                requete = "update table set number = @Number, text = @Text where number = @Number";

                connexion.Open();

                MySqlCommand commande = new MySqlCommand(requete, connexion);

                commande.Parameters.AddWithValue("@Number", Convert.ToString(List.NUMBER));
                commande.Parameters.AddWithValue("@Text", Convert.ToString(List.TEXT));

                commande.ExecuteNonQuery();

                connexion.Close();
            }
            catch (MySqlException ex)
            {
                connexion.Close();
                Console.WriteLine("Erreur PutList : " + ex.Message);
            }
        }
```

<p>Elle supprime des données dans la base de données utilisant cette méthode</p>

```
        public void DeleteList(int id)
        {
            try
            {
                requete = "delete from table where number = @Number";

                connexion.Open();

                MySqlCommand commande = new MySqlCommand(requete, connexion);

                commande.Parameters.AddWithValue("@Number", Convert.ToString(number));

                commande.ExecuteNonQuery();

                connexion.Close();
            }
            catch (MySqlException ex)
            {
                connexion.Close();
                Console.WriteLine("Erreur DeleteList " + ex.Message);
            }
        }
```

<h2 id="credits">Crédits</h2>

<p>L'application CRM Lourde a été développée par <a href="https://github.com/Str4ky">REQUISTON Timothé</a>,<br>
<a href="https://github.com/Goupil117">PEYRONNET Philippe</a> et <a href="https://github.com/mateocarciu">CARCIU Mateo</a> dans le cadre du BTS.</p>
