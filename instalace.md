# Instalace

Instalace všeho potřebného není složitá a zabere jen chvíli. Jako obvykle si ale můžeš
vybrat hned z několika možností.

> Další kroky počítají s tím, že máš nainstalovaný a funkční Python 3.
Pokud ne, návod na instalaci máme k dispozici [v začátečnickém kurzu](https://naucse.python.cz/course/pyladies/sessions/install/).

## Windows

Pokud už máš nainstalovaný Python 3 a vše bez potíží funguje, použij pro instalaci
Jupyter Notebooku [standardní cestu instalace balíčků pro Python](#instalace-pomocí-pipu).

Na Windows je možné nainstalovat Jupyter Notebook i jako součást distribuce
*Anaconda*, která mimo jiné obsahuje i Python samotný a další knihovny užitečné
zejména pro analýzu dat a výzkum. Jak na to se dozvíte [na stránkách projektu](https://www.anaconda.com/download/).

## Linux

Linuxové distribuce často mají Jupyter Notebook připraven ve formě distribučních
balíčků. Například ve Fedoře je to balíček `notebook`:

```shell
$ sudo dnf install notebook
```

V Ubuntu je instalace podobně jednoduchá:

```shell
$ sudo apt install jupyter-notebook jupyter-core
```

Pokud ve tvé distribuci Jupyter Notebook k dispozici není nebo si jej chceš
instalovat do virtuálního prostředí, přejdi na [další kapitolu](#instalace-pomocí-pipu).

## macOS

Na Macu můžeš Jupyter Notebook nainstalovat [pomocí PIPu](#instalace-pomocí-pipu),
pokud už máš nainstalovaný Python 3 a vše bez potíží funguje.

Druhou možností je použít balíčkovací nástroj [Homebrew](https://brew.sh/index_cs),
kterým jsi pravděpodobně již instalovala i samotný Python. Pokud ho nemáš, nainstaluj
si jej podle [návodu](https://brew.sh/index_cs#install).

Pokud už Homebrew v počítači máš, můžeš Jupyter Notebook nainstalovat příkazem:

```shell
$ brew install jupyter
```

## Instalace pomocí PIPu

Pokud máš Python 3 již nainstalovaný, můžeš pro instalaci balíčků použít jeho
modul jménem `pip`. Instalovat je možné buď přímo do systému, nebo do konkrétního
virtuálního prostředí. Abychom si ušetřili práci při spouštění notebooku
a abychom jej také měli k dispozici pro všechny naše projekty, nainstalujeme si
jej přímo bez aktivovaného virtuálního prostředí.

Do příkazové řádky zadej následující příkaz:

```shell
$ python3 -m pip install --user jupyter
```

> Používáš-li Windows, budeš muset pravděpodobně na začátku příkazů použít místo
`python3` jen `python`.

## Instalace ostatních knihoven

Jupyter notebook je nástroj, ve kterém budeme analýzu tvořit. Mimo nej budeme
ale potřebovat ještě:

* Pandas, což je knihovna pro zpracování dat a samotnou analýzu a
* Matplotlib, což je jedna z nejznámějších knihoven pro tvorbu grafů

Obě nainstalujeme stejným způsobem pomocí pipu:

```shell
$ python3 -m pip install --user pandas matplotlib
```

Po úspěšné instalaci by měl jít Jupyter spustit. Jak na to se dozvíš
[v následující kapitole](./jupyter&#32;notebook.md).
