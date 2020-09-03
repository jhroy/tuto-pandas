# Introduction à pandas
### Ou comment devenir un ninja des données
-----

![Logo de pandas](https://pandas.pydata.org/docs/_static/pandas.svg)
Tutoriel sur [pandas](http://pandas.pydata.org/) ([documentation](http://pandas.pydata.org/pandas-docs/stable/index.html)), bibliothèque python permettant d'analyser et d'interroger rapidement des données; particulièrement utile lorsqu'on a des fichiers volumineux qu'un tableur comme *Excel*, *Calc* ou *Google Sheets* a de la difficulté à avaler. Contenu préparé pour le [EDM5240](https://www.gitbook.com/book/jhroy/edm5240-h2017/details), cours de journalisme informatique de l'[Université du Québec à Montréal](http://uqam.ca/) (mars 2017; mis à jour en mars 2019), plus récemment changé pour [EDM4466 (Journalisme de données II)](https://journalisme-uqam.gitbook.io/edm4466-h2020/).<br>
<hr>

Le premier bloc de code, ci-dessous, ressemble au début des scripts que vous avez réalisés jusqu'à maintenant. Il s'agit d'importer les modules dont nous aurons besoin. On leur donne même un surnom. C'est ainsi que **```pandas```** devient **```pd```**, par exemple.
<br>
La ligne **```%matplotlib inline```** sert simplement à demander à notre carnet d'afficher des graphiques dans la page lorsqu'on souhaitera en créer.


```python
%matplotlib inline
import pandas as pd
import numpy as np
import matplotlib as mp
```

On peut changer les options d'affichage de pandas avec la fonction ```.set_option```.<br>
Ici, on demande que l'affichage des nombres ne soit **pas** en notation scientifique, comme il l'est par défaut.


```python
pd.options.display.float_format = "{:.2f}".format
```

Ci-dessous, on lit [deux des fichiers que je vous ai donnés](http://bit.ly/jhroypandas).<br>
On les mets chacun dans une variable. J'ai choisi de baptiser l'une de ces variables ```md``` puisque le fichier indiqué comprend des données sur l'ensemble des membres du Collège des médecins, et l'autre ```mil``` puisque le fichier indiqué contient, pour sa part, des données sur les contrats octroyés par le ministère de la Défense nationale.<br>
Pour pandas, cette structure de données, qui consiste en un tableau à deux dimensions, est appelé un _**dataframe**_.<br>


```python
md = pd.read_csv("cmq.csv")
mil = pd.read_csv("militaires.csv")
```

Pour connaître le type des variables que contient notre tableau, on peut utiliser la fonction ```.dtypes```.<p>
Dans pandas, les principaux types de variables sont&nbsp;:

* ```int``` -> nombres entiers
* ```float``` -> nombres décimaux
* ```object``` -> chaînes de caractères
* ```datetime``` -> dates
* ```bool``` -> vrai ou faux

Ces types sont parfois suivis d'un nombre qui indique la taille, en caractères, maximale des variables de ce type.


```python
md.dtypes
```




    num                object
    annee               int64
    prenom             object
    nom                object
    genre              object
    specialite1        object
    specialite2        object
    specialite3        object
    statut             object
    dateChangStatut    object
    typePermis         object
    ville              object
    prov               object
    pays               object
    dtype: object




```python
mil.dtypes
```




    annee            int64
    trimestre        int64
    date            object
    fournisseur     object
    description     object
    montant        float64
    dtype: object



## Exploration simple de nos données
-----

Pour afficher simplement le contenu de notre variable, il n'est pas nécessaire d'écrire ```print(md)```.<br>Écrire le nom de la variable suffit.<br>
Cela produit un immense tableau avec les 30 premières et les 30 dernières lignes de notre fichier.


```python
md
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>num</th>
      <th>annee</th>
      <th>prenom</th>
      <th>nom</th>
      <th>genre</th>
      <th>specialite1</th>
      <th>specialite2</th>
      <th>specialite3</th>
      <th>statut</th>
      <th>dateChangStatut</th>
      <th>typePermis</th>
      <th>ville</th>
      <th>prov</th>
      <th>pays</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>#30001</td>
      <td>1930</td>
      <td>Lucien</td>
      <td>Amyot</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1981-12-29</td>
      <td>Régulier</td>
      <td>Montréal</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>1</th>
      <td>#30002</td>
      <td>1930</td>
      <td>Wilfrid</td>
      <td>Audet</td>
      <td>M</td>
      <td>Inconnue</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Démission</td>
      <td>1987-10-01</td>
      <td>Régulier</td>
      <td>Alma</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>2</th>
      <td>#30003</td>
      <td>1930</td>
      <td>A. T.</td>
      <td>Batshaw</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1983-11-11</td>
      <td>Régulier</td>
      <td>Montréal</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>3</th>
      <td>#30005</td>
      <td>1930</td>
      <td>Maurice</td>
      <td>Beaudry</td>
      <td>M</td>
      <td>Dermatologie</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1989-02-12</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>4</th>
      <td>#30006</td>
      <td>1930</td>
      <td>P. E.</td>
      <td>Belleau</td>
      <td>M</td>
      <td>Médecine interne</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1986-05-31</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>35104</th>
      <td>#16893</td>
      <td>2016</td>
      <td>Sébastien</td>
      <td>David</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>NaN</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35105</th>
      <td>#16894</td>
      <td>2016</td>
      <td>Guillaume Patrick Jean</td>
      <td>Berthier</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Restrictif</td>
      <td>NaN</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35106</th>
      <td>#16895</td>
      <td>2016</td>
      <td>Miriam</td>
      <td>Banoub</td>
      <td>F</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>NaN</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35107</th>
      <td>#16896</td>
      <td>2016</td>
      <td>Anne-Sophie</td>
      <td>Lemay</td>
      <td>F</td>
      <td>Hématologie</td>
      <td>Oncologie médicale</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>NaN</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35108</th>
      <td>#16897</td>
      <td>2016</td>
      <td>Mohamed Ali</td>
      <td>Abla</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>NaN</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
  </tbody>
</table>
<p>35109 rows × 14 columns</p>
</div>



Pour avoir un aperçu des dimensions de de votre tableau, utilisez plutôt la fonction ```.shape```.


```python
md.shape
```




    (35109, 14)



Pour consulter les premières ou les dernières lignes de votre tableau, vous pouvez vous servir de fonctions qui ressemblent à ce qu'on a vu dans [Unix](http://bit.ly/jhroyunix), au début de la session, ```.head()``` et ```.tail()```.


```python
md.head()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>num</th>
      <th>annee</th>
      <th>prenom</th>
      <th>nom</th>
      <th>genre</th>
      <th>specialite1</th>
      <th>specialite2</th>
      <th>specialite3</th>
      <th>statut</th>
      <th>dateChangStatut</th>
      <th>typePermis</th>
      <th>ville</th>
      <th>prov</th>
      <th>pays</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>#30001</td>
      <td>1930</td>
      <td>Lucien</td>
      <td>Amyot</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1981-12-29</td>
      <td>Régulier</td>
      <td>Montréal</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>1</th>
      <td>#30002</td>
      <td>1930</td>
      <td>Wilfrid</td>
      <td>Audet</td>
      <td>M</td>
      <td>Inconnue</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Démission</td>
      <td>1987-10-01</td>
      <td>Régulier</td>
      <td>Alma</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>2</th>
      <td>#30003</td>
      <td>1930</td>
      <td>A. T.</td>
      <td>Batshaw</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1983-11-11</td>
      <td>Régulier</td>
      <td>Montréal</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>3</th>
      <td>#30005</td>
      <td>1930</td>
      <td>Maurice</td>
      <td>Beaudry</td>
      <td>M</td>
      <td>Dermatologie</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1989-02-12</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>4</th>
      <td>#30006</td>
      <td>1930</td>
      <td>P. E.</td>
      <td>Belleau</td>
      <td>M</td>
      <td>Médecine interne</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1986-05-31</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
  </tbody>
</table>
</div>




```python
mil.tail()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>annee</th>
      <th>trimestre</th>
      <th>date</th>
      <th>fournisseur</th>
      <th>description</th>
      <th>montant</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>165947</th>
      <td>2016</td>
      <td>3</td>
      <td>30-12-2016</td>
      <td>NB Harrison Inc</td>
      <td>Opérations de parachutage</td>
      <td>30700.00</td>
    </tr>
    <tr>
      <th>165948</th>
      <td>2016</td>
      <td>3</td>
      <td>30-12-2016</td>
      <td>Clint Clawson</td>
      <td>Opérations de parachutage</td>
      <td>41250.00</td>
    </tr>
    <tr>
      <th>165949</th>
      <td>2016</td>
      <td>3</td>
      <td>30-12-2016</td>
      <td>The Goodyear Tire &amp; Rubber Company</td>
      <td>Pneumatiques et chambres à air d'aéronefs</td>
      <td>282000.00</td>
    </tr>
    <tr>
      <th>165950</th>
      <td>2016</td>
      <td>3</td>
      <td>30-12-2016</td>
      <td>Imperial Oil Limited</td>
      <td>Combustible d'aviation</td>
      <td>315315.20</td>
    </tr>
    <tr>
      <th>165951</th>
      <td>2016</td>
      <td>3</td>
      <td>30-12-2016</td>
      <td>S.M.I. Support Measures Inc.</td>
      <td>Antennes, guides d'ondes et équipement connexe...</td>
      <td>630000.00</td>
    </tr>
  </tbody>
</table>
</div>



Pour consulter un intervalle précis de lignes, vous pouvez vous servir des crochets. Vous reconnaissez cette syntaxe puisque pandas, c'est du python!<br>
C'est ainsi que, ci-dessous, je demande à afficher les lignes 1000 à 1009 de mon fichier (comme en python, la limite supérieure est exclue de mon intervalle).


```python
md[1000:1010]
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>num</th>
      <th>annee</th>
      <th>prenom</th>
      <th>nom</th>
      <th>genre</th>
      <th>specialite1</th>
      <th>specialite2</th>
      <th>specialite3</th>
      <th>statut</th>
      <th>dateChangStatut</th>
      <th>typePermis</th>
      <th>ville</th>
      <th>prov</th>
      <th>pays</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1000</th>
      <td>#44048</td>
      <td>1944</td>
      <td>Paul H.</td>
      <td>Niloff</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1992-02-12</td>
      <td>Régulier</td>
      <td>Montréal</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>1001</th>
      <td>#44049</td>
      <td>1944</td>
      <td>Walter C.</td>
      <td>Lloyd-Smith</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Démission</td>
      <td>1999-07-01</td>
      <td>Régulier</td>
      <td>Sillery</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>1002</th>
      <td>#44050</td>
      <td>1944</td>
      <td>Jean-Benoit</td>
      <td>Bechard</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>2008-05-02</td>
      <td>Régulier</td>
      <td>Saint-Lambert</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>1003</th>
      <td>#44051</td>
      <td>1944</td>
      <td>H. F.</td>
      <td>Brickman</td>
      <td>F</td>
      <td>Pédiatrie</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Radié pour non-paiement de cotisation</td>
      <td>1964-08-31</td>
      <td>Régulier</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inconnu</td>
    </tr>
    <tr>
      <th>1004</th>
      <td>#44052</td>
      <td>1944</td>
      <td>E. R.</td>
      <td>Mackenzie-Harpur</td>
      <td>F</td>
      <td>Biochimie médicale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>2001-02-18</td>
      <td>Régulier</td>
      <td>Montréal</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>1005</th>
      <td>#44054</td>
      <td>1944</td>
      <td>Claude</td>
      <td>Dubé</td>
      <td>M</td>
      <td>Ophtalmologie</td>
      <td>Oto-rhino-laryngologie / chirurgie cervico-fac...</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1982-09-22</td>
      <td>Régulier</td>
      <td>Montréal</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>1006</th>
      <td>#44055</td>
      <td>1944</td>
      <td>Alban</td>
      <td>Damphousse</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1981-11-03</td>
      <td>Régulier</td>
      <td>Montréal</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>1007</th>
      <td>#44056</td>
      <td>1944</td>
      <td>James L.</td>
      <td>Mc Callum</td>
      <td>M</td>
      <td>Médecine interne</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1999-04-12</td>
      <td>Régulier</td>
      <td>Bellefeuille</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>1008</th>
      <td>#44057</td>
      <td>1944</td>
      <td>Samuel A.</td>
      <td>Macdonald</td>
      <td>M</td>
      <td>Urologie</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1995-04-02</td>
      <td>Régulier</td>
      <td>Saint-Laurent</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>1009</th>
      <td>#44061</td>
      <td>1944</td>
      <td>Léon</td>
      <td>Leclerc</td>
      <td>M</td>
      <td>Inconnue</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Démission</td>
      <td>1987-09-30</td>
      <td>Régulier</td>
      <td>Sillery</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
  </tbody>
</table>
</div>



Pour faire afficher un nombre limité de colonnes, on peut ajouter une liste du nom des colonnes qu'on souhaite.<br>
Il faut cependant le faire avec la fonction ```.loc```.


```python
md.loc[7000:7010,["nom","prenom","num"]]
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>nom</th>
      <th>prenom</th>
      <th>num</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>7000</th>
      <td>Behroozi</td>
      <td>Cyrus</td>
      <td>#67360</td>
    </tr>
    <tr>
      <th>7001</th>
      <td>Diez</td>
      <td>Garcia Pablo</td>
      <td>#67361</td>
    </tr>
    <tr>
      <th>7002</th>
      <td>Coles</td>
      <td>Duval</td>
      <td>#67362</td>
    </tr>
    <tr>
      <th>7003</th>
      <td>Pritchard</td>
      <td>Élizabeth</td>
      <td>#67363</td>
    </tr>
    <tr>
      <th>7004</th>
      <td>Braithwaite</td>
      <td>Desmond</td>
      <td>#67364</td>
    </tr>
    <tr>
      <th>7005</th>
      <td>Freeman</td>
      <td>Lincoln C.</td>
      <td>#67365</td>
    </tr>
    <tr>
      <th>7006</th>
      <td>Murat</td>
      <td>Paul</td>
      <td>#67366</td>
    </tr>
    <tr>
      <th>7007</th>
      <td>Khoury-Haddad</td>
      <td>Albert</td>
      <td>#67367</td>
    </tr>
    <tr>
      <th>7008</th>
      <td>Clecner</td>
      <td>Bya</td>
      <td>#67368</td>
    </tr>
    <tr>
      <th>7009</th>
      <td>Papapetropoulos</td>
      <td>D.</td>
      <td>#67369</td>
    </tr>
    <tr>
      <th>7010</th>
      <td>Gabriel</td>
      <td>Chafik N.</td>
      <td>#67370</td>
    </tr>
  </tbody>
</table>
</div>



On peut aussi utiliser, au lieu du nom des colonnes, le numéro d'index des colonnes qu'on souhaite afficher.<br>
Il faut alors utiliser la fonction ```.iloc```


```python
mil.iloc[100000:100011,3:]
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>fournisseur</th>
      <th>description</th>
      <th>montant</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>100000</th>
      <td>MLS USA Corporation</td>
      <td>Articles divers (Comprend seulement ces articl...</td>
      <td>158732.13</td>
    </tr>
    <tr>
      <th>100001</th>
      <td>Turtle Island Staffing</td>
      <td>Services d'aide temporaire, soutien administra...</td>
      <td>46782.00</td>
    </tr>
    <tr>
      <th>100002</th>
      <td>IMPERIAL OIL</td>
      <td>MAZOUT</td>
      <td>14329.30</td>
    </tr>
    <tr>
      <th>100003</th>
      <td>IMPERIAL OIL</td>
      <td>MAZOUT</td>
      <td>14663.55</td>
    </tr>
    <tr>
      <th>100004</th>
      <td>Valley Refrigeration Limited</td>
      <td>Travaux professionnels spéciaux de construction</td>
      <td>73989.47</td>
    </tr>
    <tr>
      <th>100005</th>
      <td>Centaur Products inc.</td>
      <td>Travaux de construction pour édifices</td>
      <td>74294.00</td>
    </tr>
    <tr>
      <th>100006</th>
      <td>Tayco Paving Company</td>
      <td>Travaux de construction - génie civil</td>
      <td>195725.00</td>
    </tr>
    <tr>
      <th>100007</th>
      <td>MCM Architects Inc.</td>
      <td>Services d'architecture et d'ingénierie - Cons...</td>
      <td>71851.00</td>
    </tr>
    <tr>
      <th>100008</th>
      <td>Shamrock Building Services Ltd</td>
      <td>Travaux de construction pour édifices</td>
      <td>168400.00</td>
    </tr>
    <tr>
      <th>100009</th>
      <td>SNC-Lavalin Environment Inc.  (Victoria)</td>
      <td>Services environnementaux</td>
      <td>71765.00</td>
    </tr>
    <tr>
      <th>100010</th>
      <td>LVM Inc.   (Montreal)</td>
      <td>Services environnementaux</td>
      <td>13731.94</td>
    </tr>
  </tbody>
</table>
</div>



Si on souhaite compter combien il y a d'éléments dans chacune de nos colonnes, on peut utiliser la fonction ```.count()```.<br>
Employons-la avec nos deux fichiers.

On constate qu'avec les médecins, il nous manque parfois de l'information. Cela peut faire du sens, comme pour les colonnes ```specialite2``` et ```specialite3```, puisque ce ne sont pas tous les médecins qui ont deux ou trois spécialités. Mais cela peut aussi vouloir dire qu'il y a des données manquantes. Ainsi, on n'a pas la ville dans laquelle excercent tous les médecins.


```python
md.count()
```




    num                35109
    annee              35109
    prenom             35108
    nom                35109
    genre              35109
    specialite1        35109
    specialite2         3467
    specialite3          224
    statut             35109
    dateChangStatut    11412
    typePermis         35109
    ville              33715
    prov               34133
    pays               35109
    dtype: int64




```python
mil.count()
```




    annee          165952
    trimestre      165952
    date           165952
    fournisseur    165952
    description    165945
    montant        165952
    dtype: int64



## Opérations sur les colonnes
-----

Il est souvent utile de connaître le nom des colonnes de notre fichier.<br>
Pour ce faire, entrez la fonction ```.columns```.


```python
md.columns
```




    Index(['num', 'annee', 'prenom', 'nom', 'genre', 'specialite1', 'specialite2',
           'specialite3', 'statut', 'dateChangStatut', 'typePermis', 'ville',
           'prov', 'pays'],
          dtype='object')



Vous remarquez que le nom de chaque colonne se trouve dans une liste. On peut se servir de cette liste pour renommer nos colonnes dans le cas où elles ont des noms barbares. Il suffit de dire que ```md.columns``` est égal à une liste dans laquelle on mettra nos nouveaux noms de colonnes.<br>
C'est ainsi que la commande ci-dessous, par exemple, me permet de rebaptiser la colonne ```dateChangStatut``` par ```date```.


```python
md.columns = ['num', 'annee', 'prenom', 'nom', 'genre', 'specialite1', 'specialite2',
       'specialite3', 'statut', 'date', 'typePermis', 'ville',
       'prov', 'pays']
```

En invoquant la fonction ```.columns```, je constate que le nom de la colonne a changé.


```python
md.columns
```




    Index(['num', 'annee', 'prenom', 'nom', 'genre', 'specialite1', 'specialite2',
           'specialite3', 'statut', 'date', 'typePermis', 'ville', 'prov', 'pays'],
          dtype='object')



Ce n'est pas le cas ici, mais il arrive fréquemment, lorsqu'on travaille avec des données ouvertes, qu'il y a beaucoup de colonnes. Cela peut rendre les données difficiles à lire, sans compter que ça peut taxer la mémoire de notre ordi. Il est possible de supprimer des colonnes contenant des informations superflues.

Si, par exemple, dans le fichier de médecins, vous souhaitiez vous débarasser de la colonne ```ville```, ce serait avec la fonction ```.drop()``` que vous vous y prendriez.

Cette fonction prend deux arguments. Le premier est la colonne (ou les colonnes) que vous souhaitez rayer de la surface de la Terre. Lorsqu'il y a plusieurs colonnes, il faut les mettre dans une liste&nbsp;: ```["colonne_1", "colonne_2", "colonne_3"]```. Le second indique si ce sont des colonnes que vous souhaitez supprimer ou des lignes. Dans le cas de colonnes, l'argument doit être ```1```, dans le cas de lignes, c'est ```0```. 


```python
md = md.drop("ville", 1)
```


```python
md.columns # La colonne «ville» a disparu!
```




    Index(['num', 'annee', 'prenom', 'nom', 'genre', 'specialite1', 'specialite2',
           'specialite3', 'statut', 'date', 'typePermis', 'prov', 'pays'],
          dtype='object')



Il est utile de simplifier les noms des colonnes puisqu'on peut faire afficher le contenu d'une colonne de notre choix simplement en ajoutant son nom à notre nom de variable.<br>
On obtient alors non plus un _**dataframe**_, mais une structure de données unidimentionnelle que pandas appelle une _**serie**_.

Voici un exemple avec le genre des médecins&nbsp;:


```python
md.genre
```




    0        M
    1        M
    2        M
    3        M
    4        M
            ..
    35104    M
    35105    M
    35106    F
    35107    F
    35108    M
    Name: genre, Length: 35109, dtype: object



## Opérations de base
-----

Cette sélection de colonnes est utile pour effectuer une série d'opérations de base qu'on va maintenant aborder.<br>
Si on a une colonne qui contient des nombres, on peut en afficher la valeur maximale ou minimale à l'aide des fonctions ```.max()``` et ```.min()```.<br>
Voici un exemple avec la colonne ```montant``` de notre fichier de données sur les contrats militaires.


```python
mil.montant.max()
```




    9975000.0




```python
mil.montant.min()
```




    0.0



On peut aussi effectuer des calculs simples sur ces colonnes.<br>
Ici, on effectue :
* une somme avec la fonction ```.sum()```
* une moyenne avec la fonction ```.mean()```

Et on trouve la médiane avec la fonction ```.median()```


```python
mil.montant.sum()
```




    27163294776.26




```python
mil.montant.mean()
```




    163681.63551063047




```python
mil.montant.median()
```




    28984.5



Dans les cas où vous avez plusieurs colonnes composées de nombres, il peut être intéressant de réunir toutes ces informations à l'intérieur d'un seul et même tableau.<br>
C'est ce que nous permet de faire la fonction ```.describe()```.


```python
mil.describe()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>annee</th>
      <th>trimestre</th>
      <th>montant</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>count</th>
      <td>165952.00</td>
      <td>165952.00</td>
      <td>165952.00</td>
    </tr>
    <tr>
      <th>mean</th>
      <td>2010.87</td>
      <td>2.57</td>
      <td>163681.64</td>
    </tr>
    <tr>
      <th>std</th>
      <td>3.27</td>
      <td>1.11</td>
      <td>595860.66</td>
    </tr>
    <tr>
      <th>min</th>
      <td>2004.00</td>
      <td>1.00</td>
      <td>0.00</td>
    </tr>
    <tr>
      <th>25%</th>
      <td>2009.00</td>
      <td>2.00</td>
      <td>15754.75</td>
    </tr>
    <tr>
      <th>50%</th>
      <td>2011.00</td>
      <td>3.00</td>
      <td>28984.50</td>
    </tr>
    <tr>
      <th>75%</th>
      <td>2014.00</td>
      <td>4.00</td>
      <td>86231.00</td>
    </tr>
    <tr>
      <th>max</th>
      <td>2016.00</td>
      <td>4.00</td>
      <td>9975000.00</td>
    </tr>
  </tbody>
</table>
</div>



## Regroupements
-----

La meilleure façon d'interroger des données est d'y effectuer différents regroupements.<br>
Dans notre fichier sur les médecins, par exemple, on a une colonne appelée ```genre``` qui nous dit si un médecin est un homme ou une femme. Cette information est représentée par deux valeurs&nbsp;: "M" ou "F".

La fonction ```value_counts()``` nous permet de compter combien il y a d'occurences de chacune de ces valeurs, donc de compter le nombre d'hommes et de femmes dans notre tableau.


```python
md.genre.value_counts()
```




    M    22441
    F    12668
    Name: genre, dtype: int64



Si on veut, plutôt, calculer le pourcentage de chacune de ces valeurs, on peut se rappeler que pandas est du bon vieux python et utiliser la fonction ```len()``` dans la formule suivante&nbsp;:


```python
md.genre.value_counts() / len(md.genre)*100
```




    M   63.92
    F   36.08
    Name: genre, dtype: float64



63,92% des médecins inscrits au tableau du Collège des médecins, donc, sont des hommes; 36,08% des femmes.

-----
On peut faire la même chose avec toutes les variables et, en combinant les fonctions ```.value_counts()``` et ```.head()```, choisir de n'afficher qu'un nombre restreint de valeurs quand on en a plusieurs. Dans notre fichier de contrats militaires, par exemple, la formule ci-dessous nous permet d'identifier quel sont les 10 fournisseurs qui ont obtenu le plus grand nombre de contrats du ministère de la Défense.


```python
mil.fournisseur.value_counts().head(10)
```




    SIMEX DEFENCE INC. / DEFENSE SIMEX INC.                         1910
    IMPERIAL OIL                                                    1608
    Unisource Technology Inc                                        1315
    FORD MOTOR COMPANY OF CANADA, LIMITED/FORD DU CANADA LIMITEE     957
    Calian Ltd                                                       950
    General Motors of Canada Limited                                 772
    J.H.T. ELECTRONICS LTD.                                          714
    BLUEWAVE ENERGY                                                  634
    WORLD FUEL SERVICES                                              628
    Imperial Oil Limited                                             601
    Name: fournisseur, dtype: int64



Vous remarquerez cependant, ici, que le 2e et le 10e fournisseur sont la même entreprise, mais écrite d'une manière différente («IMPERIAL OIL» dans un cas, «Imperial Oil Limited» dans l'autre).<br>
Ici, donc, avant d'utiliser pandas, il serait préférable d'effectuer d'abord un nettoyage de nos données avec [OpenRefine](http://openrefine.org/).
![](https://avatars0.githubusercontent.com/u/2538880?v=3&s=200)

-----

#### Nettoyage simple avec ```.str.replace()```

Si vos données ne requièrent pas de nettoyage trop complexe, vous pouvez utiliser la fonction ```.str.replace()```.

C'est l'une des nombreuses fonctions permettant de traiter du texte (chaînes de caractères ou *strings*, d'où le «.str») dans pandas.

Dans la variable ```md```, par exemple, la première colonne contient le numéro de permis de tous les médecins. Ce numéro est précédé d'un dièse ou *hashtag* (#). Vous voulez anéantir ce caractère superfétatoire. Voici comment faire.


```python
md.num = md.num.str.replace("#","")
md
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>num</th>
      <th>annee</th>
      <th>prenom</th>
      <th>nom</th>
      <th>genre</th>
      <th>specialite1</th>
      <th>specialite2</th>
      <th>specialite3</th>
      <th>statut</th>
      <th>date</th>
      <th>typePermis</th>
      <th>prov</th>
      <th>pays</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>30001</td>
      <td>1930</td>
      <td>Lucien</td>
      <td>Amyot</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1981-12-29</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>1</th>
      <td>30002</td>
      <td>1930</td>
      <td>Wilfrid</td>
      <td>Audet</td>
      <td>M</td>
      <td>Inconnue</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Démission</td>
      <td>1987-10-01</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>2</th>
      <td>30003</td>
      <td>1930</td>
      <td>A. T.</td>
      <td>Batshaw</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1983-11-11</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>3</th>
      <td>30005</td>
      <td>1930</td>
      <td>Maurice</td>
      <td>Beaudry</td>
      <td>M</td>
      <td>Dermatologie</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1989-02-12</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>4</th>
      <td>30006</td>
      <td>1930</td>
      <td>P. E.</td>
      <td>Belleau</td>
      <td>M</td>
      <td>Médecine interne</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1986-05-31</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>35104</th>
      <td>16893</td>
      <td>2016</td>
      <td>Sébastien</td>
      <td>David</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35105</th>
      <td>16894</td>
      <td>2016</td>
      <td>Guillaume Patrick Jean</td>
      <td>Berthier</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Restrictif</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35106</th>
      <td>16895</td>
      <td>2016</td>
      <td>Miriam</td>
      <td>Banoub</td>
      <td>F</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35107</th>
      <td>16896</td>
      <td>2016</td>
      <td>Anne-Sophie</td>
      <td>Lemay</td>
      <td>F</td>
      <td>Hématologie</td>
      <td>Oncologie médicale</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35108</th>
      <td>16897</td>
      <td>2016</td>
      <td>Mohamed Ali</td>
      <td>Abla</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
  </tbody>
</table>
<p>35109 rows × 13 columns</p>
</div>



#### ATTENTION

Les fonctions ```.str``` n'agissent que sur des *series*.

Ainsi, si vous écrivez la ligne de code suivante&nbsp;:

```md = md.num.str.replace("#","")```

Votre *dataframe* ```md``` va être remplacé **au complet** par une simple *serie* ne contenant que les numéros de permis des médecins.

On peut éviter ce fâcheux contretemps en demandant à ```str.replace()``` de ne transformer que la colonne ```md.num```, comme je l'ai fait quelques cellules plus haut.

-----

Dans pandas, il existe une autre fonction qui permet d'effectuer des regroupements.<br>
Il s'agit de la fonction **```.groupby()```**

On peut alors se demander quelle est la différence entre&nbsp;:

* ```mil.fournisseur.value_counts()``` et
* ```mil.groupby("fournisseur")```

La différence est simple. Il faut se souvenir que pandas travaille avec deux grandes structures de données, les *series* et les *dataframes*.

Quand on fait ```mil.fournisseur```, on crée une *series* à partir de ```mil```. C'est tout simplement une liste de valeurs. Et la fonction ```.value_counts()``` ne fait que dénombrer ces valeurs. Il faut aussi savoir que cette fonction ne s'applique qu'à des *series*.

Quand on fait ```mil.groupby("fournisseurs")``` on crée en fait autant de *dataframes* qu'il y a de fournisseurs. La fonction ```.value_counts()``` ne fonctionne plus. Mais on peut tout de même effectuer des calculs ou des regroupements en fonction des autres colonnes qui se trouvent toujours dans nos *dataframe*, une structure de données plus complexe qu'une *series*.

C'est ainsi que s'il est intéressant de connaître le nombre de contrats que chaque fournisseur a obtenu, il est encore plus pertinent de savoir qui sont les fournisseurs qui ont décroché les contrats les plus lucratifs.

La fonction ```.groupby()```, combinée à d'autres fonctions qu'on a vues antérieurement, va nous permettre de trouver la réponse.

La formule ci-dessous enchaîne cinq opérations&nbsp;:

* Un *groupby* avec ```mil``` en fonction de la colonne ```fournisseur```
* On transforme chacun des *dataframes* ainsi créés en un *serie* extrait de la colonne ```montant```
* On fait, avec la fonction ```.sum()```, la somme des montants de chacune de ces *series*
* On les ordonne en ordre décroissant avec la fonction ```.sort_values()``` et le paramètre ```ascending=**False**```
* On affiche les 10 premiers.


```python
mil.groupby("fournisseur").montant.sum().sort_values(ascending=False).head(10)
```




    fournisseur
    General Dynamics Ordnance and Tactical Systems - Canada Inc   720145247.00
    UNITED STATES DEPARTMENT OF THE NAVY (NAVAIR)                 275029944.00
    SIMEX DEFENCE INC. / DEFENSE SIMEX INC.                       225237149.00
    UNITED STATES DEPARTMENT OF THE ARMY (USASAC)                 203107502.00
    Lockheed Martin Canada Inc.                                   190692963.53
    UNITED STATES DEPARTMENT OF THE AIR FORCE (AFSAC)             154954999.00
    Calian Ltd.                                                   152633588.67
    Valcom Consulting Group Inc.                                  151766430.97
    RHEINMETALL CANADA INC.                                       140351196.40
    NATO SEASPARROW SURFACE       MISSILE SYSTEM PROJECT          125042079.00
    Name: montant, dtype: float64



## Regroupements conditionnels

On a vu, plus haut, comment sélectionner une partie d'un tableau en fonction des numéros de lignes ou de colonnes.<br>
Il est aussi possible de faire des sélections en fonction d'une valeur donnée. Par exemple, si, dans nos médecins, on souhait ne choisir que le groupe des médecins qui ont été radiés de leur ordre professionnel. On pourrait commencer par examiner la colonne ```statut``` pour voir quelles sont les différentes valeurs qu'elle contient. 


```python
md.statut.value_counts()
```




    Inscrit - Actif                                            21017
    Démission                                                   4623
    Retrait pour décès                                          3877
    Inscrit - Retraité                                          2415
    Radié pour non paiement de cotisation                       2085
    Expiration                                                   630
    Inscrit - Actif (l'exercice de ce membre est limité)         184
    Radié pour non-paiement de cotisation                         88
    Inscrit - Retraité (l'exercice de ce membre est limité)       71
    Radié                                                         67
    Retrait                                                       29
    Inscrit - Inactif                                             10
    Non inscrit                                                    9
    Révocation                                                     4
    Name: statut, dtype: int64



On remarque qu'il y a 67 médecins dont le statut est «**Radié**» et 88 dont le statut est «**Radié pour non-paiement de cotisation**». On ne s'intéresse qu'aux premiers.

On va donc créer une variable que je vais appeler ```rad``` et je vais y mettre uniquement les médecins dont le statut est «Radié» avec la formule suivante&nbsp;:


```python
rad = md.statut == "Radié"
```

Je peux maintenant utiliser le sous-ensemble ```rad``` de mon tableau ```md``` pour effectuer toutes les opérations qu'on a vues jusqu'à maintenant.<br>
Il faut seulement se souvenir que ce sous-ensemble est désigné ainsi&nbsp;: **```md[rad]```**


```python
md[rad]
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>num</th>
      <th>annee</th>
      <th>prenom</th>
      <th>nom</th>
      <th>genre</th>
      <th>specialite1</th>
      <th>specialite2</th>
      <th>specialite3</th>
      <th>statut</th>
      <th>date</th>
      <th>typePermis</th>
      <th>prov</th>
      <th>pays</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1375</th>
      <td>48004</td>
      <td>1948</td>
      <td>Alphonse</td>
      <td>Bardari</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Radié</td>
      <td>1994-10-19</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>1661</th>
      <td>49130</td>
      <td>1949</td>
      <td>Jacques</td>
      <td>Pettigrew</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Radié</td>
      <td>1993-06-17</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>2512</th>
      <td>53150</td>
      <td>1953</td>
      <td>J.-C.</td>
      <td>Paquette</td>
      <td>M</td>
      <td>Inconnue</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Radié</td>
      <td>1989-08-16</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>2761</th>
      <td>54174</td>
      <td>1954</td>
      <td>Philippe</td>
      <td>Moreault</td>
      <td>M</td>
      <td>Psychiatrie</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Radié</td>
      <td>1996-04-08</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>3057</th>
      <td>55201</td>
      <td>1955</td>
      <td>Claude</td>
      <td>Saint-Laurent</td>
      <td>M</td>
      <td>Psychiatrie</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Radié</td>
      <td>1998-07-30</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>21622</th>
      <td>93100</td>
      <td>1993</td>
      <td>Serge</td>
      <td>Grégoire</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Radié</td>
      <td>2016-05-12</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>22819</th>
      <td>95451</td>
      <td>1995</td>
      <td>Jocelyn</td>
      <td>Lussier</td>
      <td>M</td>
      <td>Pédiatrie</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Radié</td>
      <td>2009-12-21</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>23026</th>
      <td>96203</td>
      <td>1996</td>
      <td>Éric</td>
      <td>Bergeron</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Radié</td>
      <td>2016-04-28</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>24024</th>
      <td>98262</td>
      <td>1998</td>
      <td>Yves</td>
      <td>Tremblay</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Radié</td>
      <td>2016-04-30</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>27378</th>
      <td>05358</td>
      <td>2005</td>
      <td>Walif</td>
      <td>Chbeir</td>
      <td>M</td>
      <td>Radiologie diagnostique</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Radié</td>
      <td>2015-04-10</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
  </tbody>
</table>
<p>67 rows × 13 columns</p>
</div>



Je peux donc examiner quelles sont, par exemples, les spécialités les plus courantes dans le sous-ensemble des médecins radiés.


```python
md[rad].specialite1.value_counts()
```




    Inconnue                      29
    Médecine de famille           10
    Psychiatrie                    8
    Chirurgie générale             6
    Chirurgie plastique            3
    Obstétrique et gynécologie     3
    Cardiologie                    2
    Médecine interne               2
    Urologie                       1
    Radiologie diagnostique        1
    Pédiatrie                      1
    Ophtalmologie                  1
    Name: specialite1, dtype: int64



On peut également construire des sous-ensembles de façon plus souple en se basant sur la présence d'une chaîne de caractères donnés.<br>
Par exemple, dans nos contrats militaires, vous avez peut-être remarqué qu'il y en a plusieurs qui ont été octroyés à différentes composantes des forces armées américaines. Il y a entre autres&nbsp;:

* UNITED STATES DEPARTMENT OF THE ARMY
* UNITED STATES DEPARTMENT OF THE NAVY
* UNITED STATES DEPARTMENT OF THE AIR FORCE

Si on souhaite créer un sous-ensemble regroupant tous les contrats dont le nom du fournisseur contient les mots «UNITED STATES», on peut utiliser la fonction ```str.contains()``` de la façon suivante&nbsp;:


```python
us = mil.fournisseur.str.contains("UNITED STATES")
```

On peut ensuite faire un décompte des différents noms de fournisseurs qu'on a ainsi regroupés pour constater qu'il y a plusieurs agences américaines à qui la défense canadienne a octroyé des contrats.


```python
mil[us].fournisseur.value_counts()
```




    UNITED STATES DEPARTMENT OF THE ARMY (USASAC)         152
    UNITED STATES DEPARTMENT OF THE AIR FORCE (AFSAC)     131
    UNITED STATES DEPARTMENT OF THE NAVY (NAVAIR)         120
    UNITED STATES DEPARTMENT OF THE NAVY (NAVSEA)          72
    UNITED STATES DEPARTMENT OF THE AIR FORCE (AFSAT)      68
    UNITED STATES DEPARTMENT OF THE ARMY (TRADOC)          60
    UNITED STATES DEPARTMENT OF THE NAVY (NETSAFA)         55
    UNITED STATES DEPARTMENT OF THE NAVY (NAVICP)          39
    UNITED STATES DEPARTMENT OF THE NAVY (MISC)            35
    UNITED STATES DEPARTMENT OF THE NAVY (SPAWAR)          26
    UNITED STATES DEPARTMENT OF THE AIR FORCE (SAF/IA)      4
    Name: fournisseur, dtype: int64



Et quelle est la valeur totale des contrats que ces agences ont obtenu entre 2004 et 2016?


```python
mil[us].montant.sum()
```




    1069596099.0



Cette somme représente quelle proportion du total qui a été octroyé en contrats par le ministère de la Défense au cours de la même période?


```python
mil[us].montant.sum() / mil.montant.sum() * 100
```




    3.9376522907478764



#### Attention!

La fonction ```str.contains()``` est sensible à la casse. Ainsi, si on revient à nos médecins, la formule

* ```md.statut.str.contains("Actif")```

Ne donnera pas les mêmes résultats que

* ```md.statut.str.contains("actif")```


```python
actifs = md.statut.str.contains("actif")
len(md[actifs])
```




    10




```python
actifs = md.statut.str.contains("Actif")
len(md[actifs])
```




    21201



La première ne regroupe que 10 médecins, tandis que la seconde en compte 21&nbsp;201!<br>
Pourquoi?

Parce que la première ne regroupe que les médecins dont le statut contient la chaîne «actif» avec un «a» minuscule, à savoir&nbsp;:

* Inscrit - Inactif

La seconde comprend les médecins dont les statuts contiennent la même chaîne, mais avec un «A» majuscule, c'est-à-dire&nbsp;:

* Inscrit - Actif
* Inscrit - Actif (l'exercice de ce membre est limité)

-----

À partir de notre sous-ensemble de médecins actifs, on peut aussi créer d'autres sous-ensembles. La formule ci-dessous sélectionne les médecins de famille dans ce groupe.


```python
famille = md[actifs].specialite1 == "Médecine de famille"
```

Mais attention, si vous voulez afficher le sous-ensemble que vous venez de créer, vous pourriez être tenté d'écrire ceci&nbsp;:


```python
md[famille]
```

    //anaconda3/lib/python3.7/site-packages/ipykernel_launcher.py:1: UserWarning: Boolean Series key will be reindexed to match DataFrame index.
      """Entry point for launching an IPython kernel.



    ---------------------------------------------------------------------------

    IndexingError                             Traceback (most recent call last)

    <ipython-input-43-3f2f0abd82e6> in <module>
    ----> 1 md[famille]
    

    //anaconda3/lib/python3.7/site-packages/pandas/core/frame.py in __getitem__(self, key)
       2789         # Do we have a (boolean) 1d indexer?
       2790         if com.is_bool_indexer(key):
    -> 2791             return self._getitem_bool_array(key)
       2792 
       2793         # We are left with two options: a single key, and a collection of keys,


    //anaconda3/lib/python3.7/site-packages/pandas/core/frame.py in _getitem_bool_array(self, key)
       2841         # check_bool_indexer will throw exception if Series key cannot
       2842         # be reindexed to match DataFrame rows
    -> 2843         key = check_bool_indexer(self.index, key)
       2844         indexer = key.nonzero()[0]
       2845         return self._take_with_is_copy(indexer, axis=0)


    //anaconda3/lib/python3.7/site-packages/pandas/core/indexing.py in check_bool_indexer(index, key)
       2314         if mask.any():
       2315             raise IndexingError(
    -> 2316                 "Unalignable boolean Series provided as "
       2317                 "indexer (index of the boolean Series and of "
       2318                 "the indexed object do not match)."


    IndexingError: Unalignable boolean Series provided as indexer (index of the boolean Series and of the indexed object do not match).


Vous obtiendrez un message d'erreur tout aussi mystérieux qu'il peut être contrariant.

Il faut se souvenir que «famille» a été créé à partir de «actifs», il n'existe qu'en fonction du sous-ensemble ```md[actifs]```, et il faudra simplement enchaîner les deux sous-ensembles ainsi&nbsp;:


```python
md[actifs][famille]
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>num</th>
      <th>annee</th>
      <th>prenom</th>
      <th>nom</th>
      <th>genre</th>
      <th>specialite1</th>
      <th>specialite2</th>
      <th>specialite3</th>
      <th>statut</th>
      <th>date</th>
      <th>typePermis</th>
      <th>prov</th>
      <th>pays</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>4181</th>
      <td>59140</td>
      <td>1959</td>
      <td>Henri</td>
      <td>Lecoq</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif (l'exercice de ce membre est l...</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>4284</th>
      <td>59258</td>
      <td>1959</td>
      <td>Erwin B.</td>
      <td>Nichols</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Ontario</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>4384</th>
      <td>60023</td>
      <td>1960</td>
      <td>Gilles</td>
      <td>Aubin</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>4476</th>
      <td>60118</td>
      <td>1960</td>
      <td>Paul-Émile</td>
      <td>Godin</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>4481</th>
      <td>60123</td>
      <td>1960</td>
      <td>Paulin</td>
      <td>Hébert</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif (l'exercice de ce membre est l...</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>35103</th>
      <td>16892</td>
      <td>2016</td>
      <td>Steve</td>
      <td>Lauwaët</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35104</th>
      <td>16893</td>
      <td>2016</td>
      <td>Sébastien</td>
      <td>David</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35105</th>
      <td>16894</td>
      <td>2016</td>
      <td>Guillaume Patrick Jean</td>
      <td>Berthier</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Restrictif</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35106</th>
      <td>16895</td>
      <td>2016</td>
      <td>Miriam</td>
      <td>Banoub</td>
      <td>F</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35108</th>
      <td>16897</td>
      <td>2016</td>
      <td>Mohamed Ali</td>
      <td>Abla</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
  </tbody>
</table>
<p>10107 rows × 13 columns</p>
</div>



Une autre façon d'arriver exactement au même résultat est d'effectuer de façon indépendante vos deux regroupements.<br>
On pourra créer un sous-ensemble des médecins de famille à partir de l'ensemble des médecins&nbsp;:


```python
famille = md.specialite1 == "Médecine de famille"
```

Et là, écrire ```md[famille]``` va fonctionner (ce sous-ensemble regroupe 13&nbsp;150 médecins).


```python
md[famille]
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>num</th>
      <th>annee</th>
      <th>prenom</th>
      <th>nom</th>
      <th>genre</th>
      <th>specialite1</th>
      <th>specialite2</th>
      <th>specialite3</th>
      <th>statut</th>
      <th>date</th>
      <th>typePermis</th>
      <th>prov</th>
      <th>pays</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>30001</td>
      <td>1930</td>
      <td>Lucien</td>
      <td>Amyot</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1981-12-29</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>2</th>
      <td>30003</td>
      <td>1930</td>
      <td>A. T.</td>
      <td>Batshaw</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1983-11-11</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>5</th>
      <td>30008</td>
      <td>1930</td>
      <td>Antoni</td>
      <td>Blais</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1983-06-30</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>6</th>
      <td>30012</td>
      <td>1930</td>
      <td>Lyla</td>
      <td>Brown</td>
      <td>F</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1994-06-07</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>9</th>
      <td>30017</td>
      <td>1930</td>
      <td>Rémi</td>
      <td>Desjardins</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1989-09-23</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>35103</th>
      <td>16892</td>
      <td>2016</td>
      <td>Steve</td>
      <td>Lauwaët</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35104</th>
      <td>16893</td>
      <td>2016</td>
      <td>Sébastien</td>
      <td>David</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35105</th>
      <td>16894</td>
      <td>2016</td>
      <td>Guillaume Patrick Jean</td>
      <td>Berthier</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Restrictif</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35106</th>
      <td>16895</td>
      <td>2016</td>
      <td>Miriam</td>
      <td>Banoub</td>
      <td>F</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35108</th>
      <td>16897</td>
      <td>2016</td>
      <td>Mohamed Ali</td>
      <td>Abla</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
  </tbody>
</table>
<p>13150 rows × 13 columns</p>
</div>



Puis, pour faire une intersection avec nos 21&nbsp;201 médecins actifs, il vous suffira d'écrire ceci&nbsp;:


```python
md[actifs & famille]
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>num</th>
      <th>annee</th>
      <th>prenom</th>
      <th>nom</th>
      <th>genre</th>
      <th>specialite1</th>
      <th>specialite2</th>
      <th>specialite3</th>
      <th>statut</th>
      <th>date</th>
      <th>typePermis</th>
      <th>prov</th>
      <th>pays</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>4181</th>
      <td>59140</td>
      <td>1959</td>
      <td>Henri</td>
      <td>Lecoq</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif (l'exercice de ce membre est l...</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>4284</th>
      <td>59258</td>
      <td>1959</td>
      <td>Erwin B.</td>
      <td>Nichols</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Ontario</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>4384</th>
      <td>60023</td>
      <td>1960</td>
      <td>Gilles</td>
      <td>Aubin</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>4476</th>
      <td>60118</td>
      <td>1960</td>
      <td>Paul-Émile</td>
      <td>Godin</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>4481</th>
      <td>60123</td>
      <td>1960</td>
      <td>Paulin</td>
      <td>Hébert</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif (l'exercice de ce membre est l...</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>35103</th>
      <td>16892</td>
      <td>2016</td>
      <td>Steve</td>
      <td>Lauwaët</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35104</th>
      <td>16893</td>
      <td>2016</td>
      <td>Sébastien</td>
      <td>David</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35105</th>
      <td>16894</td>
      <td>2016</td>
      <td>Guillaume Patrick Jean</td>
      <td>Berthier</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Restrictif</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35106</th>
      <td>16895</td>
      <td>2016</td>
      <td>Miriam</td>
      <td>Banoub</td>
      <td>F</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35108</th>
      <td>16897</td>
      <td>2016</td>
      <td>Mohamed Ali</td>
      <td>Abla</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
  </tbody>
</table>
<p>10107 rows × 13 columns</p>
</div>



Et voilà!<br>
On sait que, dans l'ensemble des 35&nbsp;109 membres et ex-membres du Collège des médecins, on a 10&nbsp;107 médecins actifs qui sont des médecins de famille.

Maintenant, dans ce sous-groupe, quelle est la répartition homme/femme?


```python
md[famille & actifs].genre.value_counts()
```




    F    5610
    M    4497
    Name: genre, dtype: int64



Ce qui représente quelles proportions?


```python
md[famille & actifs].genre.value_counts() / len(md[famille & actifs]) * 100
```




    F   55.51
    M   44.49
    Name: genre, dtype: float64



On a peut-être une nouvelle, ici. Chez les médecins de famille actifs, au Québec, il y a une majorité de femmes (55,5%, contre 44,5% chez les hommes).

On peut même faire des sous-ensembles encore plus pointus. Par exemple, quelle est la répartition homme/femme des membres du Collège des médecins qui sont chirurgiens, actifs, ayant obtenu leur diplôme depuis 2000 et pratiquant au Québec?

On a déjà notre sous-ensemble des médecins actifs. On va en créer trois autres.

D'abord les médecins pratiquant au Québec.


```python
qc = md.prov == "Québec"
md[qc]
# Sous-ensemble de 29 794 médecins
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>num</th>
      <th>annee</th>
      <th>prenom</th>
      <th>nom</th>
      <th>genre</th>
      <th>specialite1</th>
      <th>specialite2</th>
      <th>specialite3</th>
      <th>statut</th>
      <th>date</th>
      <th>typePermis</th>
      <th>prov</th>
      <th>pays</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>30001</td>
      <td>1930</td>
      <td>Lucien</td>
      <td>Amyot</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1981-12-29</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>1</th>
      <td>30002</td>
      <td>1930</td>
      <td>Wilfrid</td>
      <td>Audet</td>
      <td>M</td>
      <td>Inconnue</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Démission</td>
      <td>1987-10-01</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>2</th>
      <td>30003</td>
      <td>1930</td>
      <td>A. T.</td>
      <td>Batshaw</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1983-11-11</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>3</th>
      <td>30005</td>
      <td>1930</td>
      <td>Maurice</td>
      <td>Beaudry</td>
      <td>M</td>
      <td>Dermatologie</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1989-02-12</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>4</th>
      <td>30006</td>
      <td>1930</td>
      <td>P. E.</td>
      <td>Belleau</td>
      <td>M</td>
      <td>Médecine interne</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1986-05-31</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>35104</th>
      <td>16893</td>
      <td>2016</td>
      <td>Sébastien</td>
      <td>David</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35105</th>
      <td>16894</td>
      <td>2016</td>
      <td>Guillaume Patrick Jean</td>
      <td>Berthier</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Restrictif</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35106</th>
      <td>16895</td>
      <td>2016</td>
      <td>Miriam</td>
      <td>Banoub</td>
      <td>F</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35107</th>
      <td>16896</td>
      <td>2016</td>
      <td>Anne-Sophie</td>
      <td>Lemay</td>
      <td>F</td>
      <td>Hématologie</td>
      <td>Oncologie médicale</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35108</th>
      <td>16897</td>
      <td>2016</td>
      <td>Mohamed Ali</td>
      <td>Abla</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
  </tbody>
</table>
<p>29794 rows × 13 columns</p>
</div>



Ensuite, les médecins ayant intégré la profession depuis 2000.<br>
Au lieu d'utiliser ```==```, on va se servir d'un autre opérateur qui peut s'appliquer à des nombres.


```python
depuis2000 = md.annee >= 2000
md[depuis2000]
# Ce sous-ensemble compte 10411 médecins
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>num</th>
      <th>annee</th>
      <th>prenom</th>
      <th>nom</th>
      <th>genre</th>
      <th>specialite1</th>
      <th>specialite2</th>
      <th>specialite3</th>
      <th>statut</th>
      <th>date</th>
      <th>typePermis</th>
      <th>prov</th>
      <th>pays</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>24698</th>
      <td>00001</td>
      <td>2000</td>
      <td>Themistocles</td>
      <td>Assimes</td>
      <td>M</td>
      <td>Médecine interne</td>
      <td>Cardiologie</td>
      <td>NaN</td>
      <td>Démission</td>
      <td>2001-07-01</td>
      <td>Régulier</td>
      <td>Californie</td>
      <td>États-Unis</td>
    </tr>
    <tr>
      <th>24699</th>
      <td>00002</td>
      <td>2000</td>
      <td>Brian</td>
      <td>Cameron</td>
      <td>M</td>
      <td>Inconnue</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Expiration</td>
      <td>2001-01-11</td>
      <td>Temporaire</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>24700</th>
      <td>00003</td>
      <td>2000</td>
      <td>François</td>
      <td>Gaumont</td>
      <td>M</td>
      <td>Médecine d'urgence</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>24701</th>
      <td>00004</td>
      <td>2000</td>
      <td>Nathalie</td>
      <td>Hache</td>
      <td>F</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>24702</th>
      <td>00005</td>
      <td>2000</td>
      <td>Geneviève</td>
      <td>Morin</td>
      <td>F</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>35104</th>
      <td>16893</td>
      <td>2016</td>
      <td>Sébastien</td>
      <td>David</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35105</th>
      <td>16894</td>
      <td>2016</td>
      <td>Guillaume Patrick Jean</td>
      <td>Berthier</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Restrictif</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35106</th>
      <td>16895</td>
      <td>2016</td>
      <td>Miriam</td>
      <td>Banoub</td>
      <td>F</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35107</th>
      <td>16896</td>
      <td>2016</td>
      <td>Anne-Sophie</td>
      <td>Lemay</td>
      <td>F</td>
      <td>Hématologie</td>
      <td>Oncologie médicale</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35108</th>
      <td>16897</td>
      <td>2016</td>
      <td>Mohamed Ali</td>
      <td>Abla</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
  </tbody>
</table>
<p>10411 rows × 13 columns</p>
</div>



Ensuite, on va identifier les chirurgiens.<br>
Ici, on va se servir de la fonction ```.str.contains()``` pour réunir tous les MD dont la spécialité contient l'expression «hirurgie», ce qui permet de repérer autant «C**hirurgie** générale» que «Neuroc**hirurgie**».


```python
chir1 = md.specialite1.str.contains("hirurgie")
md[chir1]
# On en obtient 3 259
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>num</th>
      <th>annee</th>
      <th>prenom</th>
      <th>nom</th>
      <th>genre</th>
      <th>specialite1</th>
      <th>specialite2</th>
      <th>specialite3</th>
      <th>statut</th>
      <th>date</th>
      <th>typePermis</th>
      <th>prov</th>
      <th>pays</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>7</th>
      <td>30014</td>
      <td>1930</td>
      <td>Alphonse</td>
      <td>Couturier</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1995-08-11</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>8</th>
      <td>30015</td>
      <td>1930</td>
      <td>Guy</td>
      <td>D'Argencourt</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Radié pour non-paiement de cotisation</td>
      <td>1988-11-30</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>30</th>
      <td>30063</td>
      <td>1930</td>
      <td>Arthur M.</td>
      <td>Vineberg</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>Chirurgie thoracique</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1988-03-26</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>33</th>
      <td>30072</td>
      <td>1930</td>
      <td>Maurice</td>
      <td>Berne</td>
      <td>M</td>
      <td>Oto-rhino-laryngologie / chirurgie cervico-fac...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1993-06-24</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>38</th>
      <td>30080</td>
      <td>1930</td>
      <td>C. Emerson</td>
      <td>Brooks</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Démission</td>
      <td>1977-06-30</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>35028</th>
      <td>16795</td>
      <td>2016</td>
      <td>Mohamed Akli</td>
      <td>Zetchi</td>
      <td>M</td>
      <td>Neurochirurgie</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Ontario</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35031</th>
      <td>16799</td>
      <td>2016</td>
      <td>Sara</td>
      <td>Langlais</td>
      <td>F</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35034</th>
      <td>16802</td>
      <td>2016</td>
      <td>Gabrielle</td>
      <td>Roy</td>
      <td>F</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35060</th>
      <td>16838</td>
      <td>2016</td>
      <td>Hussein</td>
      <td>Wissanji</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35061</th>
      <td>16839</td>
      <td>2016</td>
      <td>Sébastien</td>
      <td>Lachance</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
  </tbody>
</table>
<p>3259 rows × 13 columns</p>
</div>



Il faut également vérifier les médecins dont la 2e ou 3e spécialité est la chirurgie, car on a trois colonnes de spécialités.<br>
Il faudra cependant ajouter un paramètre à la fonction ```.str.contains``` qui va faire en sorte d'ignorer les médecins qui n'ont aucune 2e ou 3e spécialité avec l'argument ```na=False```.


```python
chir2 = md.specialite2.str.contains("hirurgie", na=False)
md[chir2]
# On obtient ici 268 médecins
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>num</th>
      <th>annee</th>
      <th>prenom</th>
      <th>nom</th>
      <th>genre</th>
      <th>specialite1</th>
      <th>specialite2</th>
      <th>specialite3</th>
      <th>statut</th>
      <th>date</th>
      <th>typePermis</th>
      <th>prov</th>
      <th>pays</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>19</th>
      <td>30042</td>
      <td>1930</td>
      <td>Marcel</td>
      <td>Ostiguy</td>
      <td>M</td>
      <td>Ophtalmologie</td>
      <td>Oto-rhino-laryngologie / chirurgie cervico-fac...</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1994-10-15</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>30</th>
      <td>30063</td>
      <td>1930</td>
      <td>Arthur M.</td>
      <td>Vineberg</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>Chirurgie thoracique</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1988-03-26</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>69</th>
      <td>31050</td>
      <td>1931</td>
      <td>Gérard</td>
      <td>Rolland</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>Chirurgie thoracique</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1989-10-28</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>74</th>
      <td>31059</td>
      <td>1931</td>
      <td>L. J.</td>
      <td>Tessier</td>
      <td>M</td>
      <td>Ophtalmologie</td>
      <td>Oto-rhino-laryngologie / chirurgie cervico-fac...</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>2002-12-26</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>99</th>
      <td>32011</td>
      <td>1932</td>
      <td>J. A.</td>
      <td>Bohemier</td>
      <td>M</td>
      <td>Ophtalmologie</td>
      <td>Oto-rhino-laryngologie / chirurgie cervico-fac...</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1996-04-01</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>31776</th>
      <td>12698</td>
      <td>2012</td>
      <td>Heather</td>
      <td>Gill</td>
      <td>F</td>
      <td>Chirurgie générale</td>
      <td>Chirurgie vasculaire</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>32003</th>
      <td>13111</td>
      <td>2013</td>
      <td>Dominique</td>
      <td>Boudreau</td>
      <td>F</td>
      <td>Chirurgie générale</td>
      <td>Chirurgie générale oncologique</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>33100</th>
      <td>14430</td>
      <td>2014</td>
      <td>Mireille</td>
      <td>Méthot</td>
      <td>F</td>
      <td>Chirurgie générale</td>
      <td>Chirurgie vasculaire</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>33151</th>
      <td>14481</td>
      <td>2014</td>
      <td>Ricardo</td>
      <td>Ruz</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>Chirurgie vasculaire</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>34481</th>
      <td>16207</td>
      <td>2016</td>
      <td>Mai-Kim</td>
      <td>Gervais</td>
      <td>F</td>
      <td>Chirurgie générale</td>
      <td>Chirurgie générale oncologique</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
  </tbody>
</table>
<p>268 rows × 13 columns</p>
</div>




```python
chir3 = md.specialite3.str.contains("hirurgie", na=False)
md[chir3]
# Quatre médecins dans ce sous-ensemble
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>num</th>
      <th>annee</th>
      <th>prenom</th>
      <th>nom</th>
      <th>genre</th>
      <th>specialite1</th>
      <th>specialite2</th>
      <th>specialite3</th>
      <th>statut</th>
      <th>date</th>
      <th>typePermis</th>
      <th>prov</th>
      <th>pays</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>313</th>
      <td>36013</td>
      <td>1936</td>
      <td>J. Ernest</td>
      <td>Bousquet</td>
      <td>M</td>
      <td>Chirurgie thoracique</td>
      <td>Pneumologie</td>
      <td>Chirurgie générale</td>
      <td>Retrait pour décès</td>
      <td>1983-11-06</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>10671</th>
      <td>74293</td>
      <td>1974</td>
      <td>Pierre</td>
      <td>Michaud</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>Chirurgie thoracique</td>
      <td>Chirurgie vasculaire</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>12161</th>
      <td>76365</td>
      <td>1976</td>
      <td>Louise</td>
      <td>Choiniere</td>
      <td>F</td>
      <td>Chirurgie générale</td>
      <td>Chirurgie cardio-vasculaire et thoracique</td>
      <td>Chirurgie thoracique</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>16006</th>
      <td>82154</td>
      <td>1982</td>
      <td>Rosaire</td>
      <td>Vaillancourt</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>Chirurgie cardio-vasculaire et thoracique</td>
      <td>Chirurgie thoracique</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
  </tbody>
</table>
</div>



Si on veut les réunir tous et y voir la répartition homme/femme, la formule ci-dessous les combine de la façon suivante&nbsp;:

Médecins actifs **ET**<br>
pratiquant au Québec **ET**<br>
depuis 2000 **ET**<br>
dont la spécialité&nbsp;1 **OU** la spécialité&nbsp;2 **OU** la spécialité&nbsp;3 est une forme ou une autre de chirurgie.


```python
md[actifs & qc & depuis2000 & (chir1 | chir2 | chir3)].genre.value_counts()
```




    M    482
    F    280
    Name: genre, dtype: int64



Au tout début de notre carnet, on a importé cette bibliothèque au nom affeux, **matplotlib**.<br>
On va s'en servir pour créer des graphiques. Pour ce faire, il suffit d'ajouter la fonction ```.plot()``` à la fin d'une formule.


```python
md[famille & actifs].genre.value_counts().plot()
```




    <matplotlib.axes._subplots.AxesSubplot at 0x118e64278>




![png](output_117_1.png)


Ce n'est pas très évocateur. On peut heureusement changer le type de graphique pour, par exemple, choisir un graphique en pointes de tarte. Il suffit d'ajouter, à la fonction ```.plot()``` l'argument ```kind``` auquel on donne la valeur de ```pie```.<br>
On peut aussi donner un titre à notre graphique avec l'argument ```title```.


```python
md[famille & actifs].genre.value_counts().plot(kind="pie", title="Majorité de femmes médecin de famille au Québec")
```




    <matplotlib.axes._subplots.AxesSubplot at 0x118ea5198>




![png](output_119_1.png)


Un autre type de graphique intéressant est l'histogramme.<br>
Pour tracer l'évolution du nombre de médecins ayant intégré la profession médicale au cours des ans, on pourrait faire un histogramme de notre tableau ```md``` en fonction de la colonne ```annee``` avec la formule suivante&nbsp;:


```python
md.annee.hist()
```




    <matplotlib.axes._subplots.AxesSubplot at 0x1172bc4e0>




![png](output_121_1.png)


Mais voilà qui ne raconte pas grand-chose. C'est que par défaut, l'histogramme trace 10 barres, ce qui fait que chaque barre de notre histogramme regroupe 7 ou 8 années.<br>
Les barres, c'est que ce matplotlib appelle des *«bins»*. On peut ainsi spécifier le nombre de ces *bins* avec un argument qui s'appelle... vous l'aurez deviné... ```bins```

Ici, comme nos données couvrent 87 années, on va créer 87 barres.<br>
Chacune représente le nombre de médecins qui ont obtenu leur permis de pratique au cours d'une année donnée.


```python
md.annee.hist(bins=87)
```




    <matplotlib.axes._subplots.AxesSubplot at 0x1194ec940>




![png](output_123_1.png)


Il remarque une chute au début des années 1990. Elle correspond à une politique du gouvernement québécois qui avait limité le nombre d'inscriptions dans les facultés de médecine quelques années auparavant.

Inspiré par ce graphique, vous pourriez avoir envie de voir combien d'hommes et de femmes sont devenus médecin au fil des ans afin de visualiser la féminisation de la profession médicale. Pour ce faire, il suffirait de modifier la formule ci-dessus en ajoutant un ```groupby``` par ```genre```, puis l'argument ```alpha``` à la fonction ```.hist()``` pour faire en sorte que nos barres aient une transparence de 50%.


```python
md.groupby("genre").annee.hist(bins=87,alpha=0.5)
```




    genre
    F    AxesSubplot(0.125,0.125;0.775x0.755)
    M    AxesSubplot(0.125,0.125;0.775x0.755)
    Name: annee, dtype: object




![png](output_125_1.png)


Le graphique ci-dessus raconte une histoire avec les données.

On y voit que jusqu'en 1970, les hommes (en jaune) étaient clairement majoritaires dans la profession.<br>
À partir de 1970 semble s'opérer un renversement. Le nombre d'hommes diminue progressivement pour, dès 1990, devenir inférieur au nombre de femmes (en bleu).<br>
Aujourd'hui, les deux tiers des recrues, en médecine, chaque année, sont des femmes.

-----

En terminant, faisons aussi un graphique avec nos données de contrats.<br>
Calculons la somme des contrats octroyés chaque année, créons un diagramme à barres horizontales (```kind="barh"```) et donnons une couleur de camouflage (*teal*) à nos barres.


```python
mil.groupby("annee").montant.sum().plot(kind="barh",color="teal")
```




    <matplotlib.axes._subplots.AxesSubplot at 0x1175088d0>




![png](output_128_1.png)


#### Voilà! J'espère que, grâce à pandas, vous aurez un peu de plaisir à explorer vos données!


```python

```
