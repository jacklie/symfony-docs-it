La squadra di Symfony
=====================

Questo documento elenca le regole che governano la squadra di Symfony. Tali regole
sono effettive a partire dalla pubblicazione di questo documento e tutti i membri della squadra di Symfony
devono rispettarle.

Organizzazione
--------------

I membri della squadra di Symfony sono divisi in tre gruppi. Ciascun membro può appartenere
a un solo gruppo alla volta. I privilegi garantiti a un gruppo sono automaticamente estesi
a ogni gruppo che abbia priorità maggiore.

I gruppi della squadra di Symfony, in ordine decrescente di priorità, sono i seguenti:

1. **Capo progetto**

* Elegge i membri degli altri gruppi;
* Esegue i merge delle richieste di pull in tutti i repoistory di Symfony.

2. **Merger**

* Eseguono i merge delle richieste di pull per i componenti che sono stati
  loro assegnati.

3. **Decider**

* Decidono per un merge o un rifiuto di una richiesta di pull.

Membri attivi
~~~~~~~~~~~~~

.. role:: leader
.. role:: merger
.. role:: decider

* **Capo progetto**:

  * **Fabien Potencier** (:leader:`fabpot`).

* **Merger**:

  * **Bernhard Schussek** (:merger:`webmozart`) per i componenti Form_,
    Validator_, Icu_, Intl_, Locale_, OptionsResolver_ e PropertyAccess_;


  * **Tobias Schultze** (:merger:`Tobion`) per il componente Routing_;


  * **Romain Neutron** (:merger:`romainneutron`) per il componente
    Process_;

  * **Nicolas Grekas** (:merger:`nicolas-grekas`) per il componente Debug_.


  * **Christophe Coevoet** (:merger:`stof`) per i componenti BrowserKit_,
    Config_, Console_, DependencyInjection_, DomCrawler_, EventDispatcher_,
    HttpFoundation_, HttpKernel_, Serializer_, Stopwatch_, DoctrineBridge_,
    MonologBridge_, e TwigBridge_.

  * **Kévin Dunglas** (:merger:`dunglas`) per il componente Serializer_.


* **Decider**:

  * **Jakub Zalas** (:decider:`jakzal`);
  * **Jordi Boggiano** (:decider:`seldaek`);
  * **Lukas Kahwe Smith** (:decider:`lsmith77`);
  * **Ryan Weaver** (:decider:`weaverryan`).

Richiesta di affiliazione
~~~~~~~~~~~~~~~~~~~~~~~~~

Al momento non si accettano richieste di nuovi membri per la squadra di Symfony.

Revoca dall'affiliazione
~~~~~~~~~~~~~~~~~~~~~~~~

Un membro della squadra di Symfony può essere espulso per una delle seguenti ragioni:

* Rifiuto di seguire le regole elencate in questo documento;
* Mancanza di attività nei sei mesi precedenti;
* Negligenza deliberata o intenzione di danneggiare il progetto Symfony;
* Su decisione del **capo progetto**.

Se in futuro saranno accettati nuovi membri, i membri espulsi
dovranno attendere dodici mesi prima di richiedere una riammissione.

Regole sullo sviluppo del codice
--------------------------------

Lo sviluppo del progetto Symfony si basa su richieste di pull, proposte da qualsiasi membro
della comunità di Symfony. L'accettazione o il rifiuto delle richieste di pull sono decisi in base
ai voti espressi dai membri della squadra di Symfony.

Votazione delle richieste di pull
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

* I voti ``-1`` vanno sempre giustificati con ragioni tecniche e oggettive;

* I voti ``+1`` non richiedono giustificazioni, a meno che non ci sia almeno un
  voto ``-1``;

* I membri della squadra possono modificare i propri voti in qualsiasi momento, nel
  corso della discussione su una richiesta di pull;

* Un membro della squadra non può votare una sua richiesta di pull.

Merge delle richieste di pull
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Si può eseguire il merge di una richiesta di pull se:

* Sia passato abbastanza tempo per le revisioni (alcuni minuti per le modifiche
  minori, almeno due giorni per le richieste di pull "normali" e quattro giorni per
  le richieste di pull con "impatto significativo");

* Sia una modifica minore [1]_, indipendentemente dal numero di voti;

* Almeno il **merger** del componente o altri due membri della squadra abbiano votato ``+1``
  e nessun altro membro abbia votato ``-1``.

Processo di merge delle richieste di pull
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Tutto il codice deve passare per richieste di pull, tranne le
modifiche minori [1]_, che possono essere committate direttamente nel repository.

I **merger** devono usare sempre lo strumento ``gh``, fornito dal
**capo progetto**, per il merge delle richieste di pull.

Rilasci
~~~~~~~

Il **capo progetto** è anche il gestore dei rilasci di ogni versione di Symfony.

Emendamenti alle regole
-----------------------

Le regole descritte in questo documento potranno essere emendate in qualsiasi momento,
a discrezione del **capo progetto**.


.. [1] Le modifiche minori includono errori di battitura, sistemazioni di DocBlock, violazioni
       agli standard del codice, modifiche minori a CSS, JavaScript e HTML.

.. _BrowserKit: https://github.com/symfony/BrowserKit
.. _Config: https://github.com/symfony/Config
.. _Console: https://github.com/symfony/Console
.. _Debug: https://github.com/symfony/Debug
.. _DependencyInjection: https://github.com/symfony/DependencyInjection
.. _DoctrineBridge: https://github.com/symfony/DoctrineBridge
.. _EventDispatcher: https://github.com/symfony/EventDispatcher
.. _DomCrawler: https://github.com/symfony/DomCrawler
.. _Form: https://github.com/symfony/Form
.. _HttpFoundation: https://github.com/symfony/HttpFoundation
.. _HttpKernel: https://github.com/symfony/HttpKernel
.. _Icu: https://github.com/symfony/Icu
.. _Intl: https://github.com/symfony/Intl
.. _Locale: https://github.com/symfony/Locale
.. _MonologBridge: https://github.com/symfony/MonologBridge
.. _OptionsResolver: https://github.com/symfony/OptionsResolver
.. _Process: https://github.com/symfony/Process
.. _PropertyAccess: https://github.com/symfony/PropertyAccess
.. _Routing: https://github.com/symfony/Routing
.. _Serializer: https://github.com/symfony/Serializer
.. _Stopwatch: https://github.com/symfony/Stopwatch
.. _TwigBridge: https://github.com/symfony/TwigBridge
.. _Validator: https://github.com/symfony/Validator
