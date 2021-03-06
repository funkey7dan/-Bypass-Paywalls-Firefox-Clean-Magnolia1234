# Bypass Paywalls Clean for Firefox

Add-on allows you to read articles from (supported) sites that implement a paywall.  
You can also add domains as custom site and try to bypass the paywall.  
Weekly updates are released for fixes and new sites.

* [Installation](#installation)
* [Update](#update)
* [List of supported websites](#list-of-supported-websites)
* [Sites with limited number of free articles](#sites-with-limited-number-of-free-articles)
* [New site requests](#new-site-requests)
* [Add custom site](#add-custom-site)
* [Add excluded site](#add-excluded-site)
* [Troubleshooting](#troubleshooting)
* [Changelog-releases](#changelog-releases)
* [License](#license)
* [Disclaimer](#disclaimer)

### Installation
You can install the add-on from Mozilla add-ons (AMO): [Bypass Paywalls Clean](https://addons.mozilla.org/en-US/firefox/addon/bypass-paywalls-clean)\
Latest add-on versions (2.4.8.0+) require a browser based on Firefox 86+ (else use the non-amo version below).\
Or download and install the latest xpi-version from [GitLab](https://gitlab.com/magnolia1234/bypass-paywalls-firefox-clean/-/releases)

If you want to install the latest [master ZIP-file from GitLab](https://gitlab.com/magnolia1234/bypass-paywalls-firefox-clean/-/archive/master/bypass-paywalls-firefox-clean-master.zip) use a Firefox browser which allows using unsigned add-ons like Firefox Developer Portable (go to about:config and set xpinstall.signatures.required to false) or LibreWolf (for both no automatic updates of add-on).\
Or load a temporary add-on in regular Firefox (go to about:debugging#/runtime/this-firefox & load manifest.json from unpacked folder (of master-zip)).

By default BPC has limited permissions, but you can opt-in to enable custom sites (and also clear cookies/block general paywall-scripts for non-listed sites). You can also just request permissions for the custom sites you added yourself (or click `clear cookies` (BPC-icon) to ask for permission for current site).

### Update
Check for updates (in about:addons) and allow permissions for newly supported sites (else no update will be installed).\
You can also check for update of site rules at startup (opt-in).\
For new sites you also have to opt-in to custom sites/request permissions for new domains (or wait for new release).

#### Android
On Android this add-on doesn't work with latest Firefox v84 (Fenix); it only supports a number of 'recommended' add-ons (for now).\
Only from Firefox v85 you can install recommended add-ons via [AMO](https://addons.mozilla.org) - so no more need to add these to your custom add-on collection (see below).

BPC add-on works fine in [Firefox Nightly](https://play.google.com/store/apps/details?id=org.mozilla.fenix), [Fennec F-Droid](https://f-droid.org/en/packages/org.mozilla.fennec_fdroid) or [IceRaven](https://github.com/fork-maintainers/iceraven-browser) though (when you load BPC from a [custom add-on collection](https://blog.mozilla.org/addons/2020/09/29/expanded-extension-support-in-firefox-for-android-nightly)).\
For Firefox Nightly or Fennec F-Droid (based on latest Firefox for Android) you have to make your own custom add-on collection (or use another that contains BPC). \
[Iceraven (Fenix fork)](https://github.com/fork-maintainers/iceraven-browser) uses: [What I want on Fenix](https://addons.mozilla.org/en-US/firefox/collections/16201230/What-I-want-on-Fenix)\
It has a custom add-ons account: 16201230 & collection: What-I-want-on-Fenix.\
In IceRaven all add-ons are shown (with search option), but In Firefox Nightly and Fennec F-Droid only the first 50 add-ons are shown.\
There you can use custom add-ons account: 15546469 & collection: Fenix.

PS on Android: enabling custom sites isn't working (no optional permissions).\
Then you need the 'custom' add-on version (with access to all sites): [Bypass Paywalls Clean (custom)](https://addons.mozilla.org/en-US/firefox/addon/bypass-paywalls-clean-custom)

#### Chrome/Chromium
Visit the [Chrome repository](https://gitlab.com/magnolia1234/bypass-paywalls-chrome-clean) of Bypass Paywall Clean.

#### iOS/iPadOS
Use adblocker with custom (content)filter: https://gitlab.com/magnolia1234/bypass-paywalls-clean-filters

#### Notes
* This add-on works best alongside the adblocker [uBlock Origin](https://addons.mozilla.org/en-US/firefox/addon/ublock-origin).
* You will be logged out for most of the sites you have checked.
* Some sites need to redirect to an amp-page (add an exception in your `Redirect AMP to HTML` add-on).

### List of supported websites

_* free/cached articles only._

##### World news
[Foreign Affairs](https://www.foreignaffairs.com) -
[Foreign Policy](https://www.foreignpolicy.com) -
[Harper's Magazine](https://harpers.org) -
[Inkl](https://www.inkl.com) -
[Newsweek](https://www.newsweek.com) -
[Reuters](https://www.reuters.com) -
[Stratfor](https://stratfor.com) -
[The American Interest](https://www.the-american-interest.com) -
[The Atlantic](https://www.theatlantic.com) -
[The Christian Science Monitor](https://www.csmonitor.com) -
[The Nation](https://www.thenation.com) -
[The New Republic](https://newrepublic.com) -
[The New York Review of Books](https://www.nybooks.com) -
[The New York Times](https://www.nytimes.com) -
[The Spectator World](https://spectatorworld.com) -
[The Washington Post](https://www.washingtonpost.com) -
[Time Magazine](https://time.com) -
[World Politics Review](https://www.worldpoliticsreview.com)

##### Business
[Adweek](https://www.adweek.com)* -
[American Affairs](https://americanaffairsjournal.org) -
[American Banker](https://www.americanbanker.com) -
[Barron's](https://www.barrons.com) -
[Bloomberg](https://www.bloomberg.com) -
[Business Insider](https://www.businessinsider.com) -
[Digiday](https://digiday.com) -
[Entrepreneur](https://www.entrepreneur.com) -
[Forbes](https://www.forbes.com) -
[Fortune](https://fortune.com) -
[Harvard Business Review](https://www.hbr.org) -
[Inc.com](https://www.inc.com) -
[Law.com](https://www.law.com)* -
[Law360](https://www.law360.com)* -
[MarketWatch](https://www.marketwatch.com) -
[MIT Sloan Management Review](https://sloanreview.mit.edu) -
[Quartz](https://qz.com) -
[S&P Global](https://www.spglobal.com) -
[Seeking Alpha](https://seekingalpha.com) -
[Stock News](https://stocknews.com) -
[The Business Journals](https://www.bizjournals.com) -
[The Business of Fashion](https://www.businessoffashion.com) -
[The Wall Street Journal](https://www.wsj.com) -
[Vogue Business](https://www.voguebusiness.com)

Grouped in options:\
*Crain Communications* sites like\
[Ad Age](https://adage.com) -
[Automotive News](https://www.autonews.com) -
[Crain's Chicago Business](https://www.chicagobusiness.com) -
[Crain's Cleveland Business](https://www.crainscleveland.com) -
[Crain's Detroit Business](https://www.crainsdetroit.com) -
[Crain's New York Business](https://www.crainsnewyork.com) -
[Modern Healthcare](https://www.modernhealthcare.com)\
*NHST Media Group* sites like\
[Intrafish](https://www.intrafish.com) -
[Recharge](https://www.rechargenews.com) -
[TradeWinds](https://www.tradewindsnews.com) -
[Upstream](https://www.upstreamonline.com)

##### Tech/Science
[360Dx](https://www.360dx.com) -
[Chemical & Engineering News](https://cen.acs.org) -
[Chronicle of Higher Education](https://www.chronicle.com) -
[Dark Reading](https://www.darkreading.com) -
[Discover Magazine](https://www.discovermagazine.com) -
[GenomeWeb](https://www.genomeweb.com) -
[MIT Technology Review](https://www.technologyreview.com) -
[National Geographic USA](https://www.nationalgeographic.com) -
[Nautilus](https://nautil.us) -
[Precision Oncology News](https://www.precisiononcologynews.com) -
[Science](https://www.science.org)* -
[Scientific American](https://www.scientificamerican.com)* -
[Times Higher Education](https://www.timeshighereducation.com) -
[VentureBeat](https://venturebeat.com)

##### Encyclopedia/Book library/Knowledge base
[BBC History Extra](https://www.historyextra.com) -
[Encyclopedia Britannica](https://www.britannica.com) -
[eNotes](https://www.enotes.com) -
[Glassdoor](https://www.glassdoor.com) -
[Loeb Classical Library](https://www.loebclassics.com) -
[Philosophy Now](https://philosophynow.org) -
[Quora](https://www.quora.com) -
[Scribd](https://www.scribd.com) -
[Statista](https://www.statista.com) -
[Study.com (no videos)](https://study.com)

##### Magazines/Blogs
[Medium](https://www.medium.com)*\
Grouped in options:\
*Medium custom domains* like (opt-in to custom sites for unlisted):\
[Better Programming](https://betterprogramming.pub) -
[Towards Data Science](https://towardsdatascience.com)

[Apollo Magazine](https://www.apollo-magazine.com) -
[Artnet](https://www.artnet.com) -
[Atavist Magazine](https://magazine.atavist.com) -
[Commentary Magazine](https://www.commentary.org) -
[ESPN USA](https://www.espn.com) -
[First Things](https://www.firstthings.com) -
[National Review](https://www.nationalreview.com) -
[Puck.news](https://puck.news) -
[RugbyPass](https://www.rugbypass.com) -
[Slate](https://slate.com) -
[SofRep](https://sofrep.com) -
[Sports Illustrated](https://www.si.com) -
[The Art Newspaper](https://www.theartnewspaper.com) -
[The Athletic](https://theathletic.com) -
[The Intercept](https://theintercept.com) -
[The Daily Beast](https://www.thedailybeast.com) -
[The Daily Wire](https://www.dailywire.com) -
[The New Atlantis](https://www.thenewatlantis.com) -
[The Point Magazine](https://thepointmag.com) -
[The Wrap](https://www.thewrap.com)

Grouped in options:\
*Cond?? Nast magazines* sites like:\
[Bon App??tit](https://www.bonappetit.com) -
[GC](https://www.gq.com) -
[The New Yorker](https://www.newyorker.com) -
[Vanity Fair](https://www.vanityfair.com) -
[Vogue USA](https://www.vogue.com) -
[Wired](https://www.wired.com)\
*Hearst Communications magazines* sites like:\
[Bicycling](https://www.bicycling.com) -
[Cosmopolitan](https://www.cosmopolitan.com) -
[Country Living](https://www.countryliving.com) -
[Elle USA](https://www.elle.com) -
[Esquire](https://www.esquire.com) -
[Good Housekeeping](https://www.goodhousekeeping.com) -
[House Beautiful](https://www.housebeautiful.com) -
[Men's Health](https://www.menshealth.com) -
[Popular Mechanics](https://www.popularmechanics.com) -
[Prevention](https://www.prevention.com) -
[Road & Track](https://www.roadandtrack.com) -
[Runner's World](https://www.runnersworld.com) -
[The Hollywood Reporter](https://www.hollywoodreporter.com) -
[Town & Country](https://www.townandcountrymag.com) -
[Women's Health](https://www.womenshealthmag.com)\
*Outside magazines* sites like:\
[Backpacker](https://www.backpacker.com) -
[Beta](https://www.betamtb.com) -
[Better Nutrition](https://www.betternutrition.com) -
[Clean Eating](https://www.cleaneatingmag.com) -
[Climbing](https://www.climbing.com) -
[Cycling Tips](https://cyclingtips.com) -
[Gym Climber](https://www.gymclimber.com) -
[Outside](https://www.outsideonline.com) -
[Oxygen](https://www.oxygenmag.com) -
[Peloton](https://www.pelotonmagazine.com) -
[Podium Runner](https://www.podiumrunner.com) -
[Rock and Ice](https://www.rockandice.com) -
[SKI](https://www.skimag.com) -
[Trail Runner](https://www.trailrunnermag.com) -
[Triathlete](https://www.triathlete.com) -
[Vegetarian Times](https://www.vegetariantimes.com) -
[Velo News](https://www.velonews.com) -
[Women's Running](https://www.womensrunning.com) -
[Yoga Journal](https://www.yogajournal.com)\
*Penske Media Corporation* sites like:\
[Billboard](https://www.billboard.com) -
[Rolling Stone](https://www.rollingstone.com) -
[Sportico](https://www.sportico.com) -
[Variety](https://variety.com) -
[WWD](https://wwd.com)

##### Local USA news
[Honolulu Star-Advertiser](https://www.staradvertiser.com) -
[Los Angeles Business Journal](https://labusinessjournal.com) -
[Los Angeles Times](https://www.latimes.com) -
[Mountain View Voice](https://www.mv-voice.com) -
[New York Magazine](https://www.nymag.com) (+ [Curbed](https://www.curbed.com), [Grub Street](https://www.grubstreet.com), [The Cut](https://www.thecut.com) & [Vulture](https://www.vulture.com)) -
[Newsday](https://www.newsday.com) -
[Palo Alto Online](https://www.paloaltoonline.com) -
[Pittsburgh Post Gazette](https://www.post-gazette.com) -
[San Diego Union Tribune](https://www.sandiegouniontribune.com) -
[Star Tribune](https://www.startribune.com) -
[Tampa Bay Times](https://www.tampabay.com) -
[The Advocate](https://www.theadvocate.com) -
[The Atlanta Journal-Constitution](https://www.ajc.com) -
[The Boston Globe](https://www.bostonglobe.com) -
[The Dallas Morning News](https://www.dallasnews.com) -
[The New Orleans Advocate/The Times-Picayune](https://www.nola.com) -
[The Seattle Times](https://www.seattletimes.com) -
[The Philadelphia Inquirer](https://www.inquirer.com)

[USA Today](https://www.usatoday.com)\
Grouped in options:\
*Advance Local* sites like:\
[AL/Alabama](https://www.al.com) -
[MLive/Michigan](https://www.mlive.com) -
[NJ/New Jersey](https://www.nj.com) -
[Staten Island Advance](https://www.silive.com) -
[The Express-Times](https://www.lehighvalleylive.com) -
[The Oregonian](https://www.oregonlive.com) -
[The Patriot-News](https://www.pennlive.com) -
[The Plain Dealer](https://www.cleveland.com) -
[The Post-Standard](https://www.syracuse.com) -
[The Republican](https://www.masslive.com)\
*Gannett Group (local USA Today)* sites like (opt-in to custom sites for unlisted)\
[Austin American-Statesman](https://www.statesman.com) -
[Detroit Free Press](https://www.freep.com) -
[Milwaukee Journal Sentinel](https://www.jsonline.com) -
[The Arizona Republic](https://www.azcentral.com) -
[The Cincinnati Enquirer](http://www.cincinnati.com) -
[The Courier-Journal](https://www.courier-journal.com) -
[The Detroit News](https://www.detroitnews.com) -
[The Indianapolis Star](https://www.indystar.com) -
[The Record (North Jersey)](https://www.northjersey.com) -
[The Tennessean](http://www.tennessean.com)\
*Hearst Communications (newspapers)* sites like (opt-in to custom sites for unlisted)\
[Houston Chronicle](https://www.houstonchronicle.com) -
[San Antonio Express-News](https://www.expressnews.com) -
[San Francisco Chronicle](https://www.sfchronicle.com)\
*Lee Enterprises Group* sites like (opt-in to custom sites for unlisted)\
[Arizona Daily Star](https://tucson.com) -
[Richmond Times-Dispatch](https://richmond.com) -
[The Buffalo News](https://buffalonews.com) -
[Tulsa World](https://tulsaworld.com) -
[Winston-Salem Journal](https://www.journalnow.com)\
*McClatchy Group* sites like (opt-in to custom sites for unlisted)\
[Belleville News-Democrat](https://www.bnd.com) -
[Fort Worth Star-Telegram](https://www.star-telegram.com) -
[Lexington Herald-Leader](https://www.kentucky.com) -
[Miami Herald](https://www.miamiherald.com) -
[The Charlotte Observer](https://www.charlotteobserver.com) -
[The Fresno Bee](https://www.fresnobee.com) -
[The Kansas City Star](https://www.kansascity.com) -
[The News & Observer](https://www.newsobserver.com) -
[The Sacramento Bee](https://www.sacbee.com) -
[The State](https://www.thestate.com) -
[The Wichita Eagle](https://www.kansas.com) -
[Tri-City Herald](https://www.tri-cityherald.com)\
*MediaNews Group* sites like (opt-in to custom sites for unlisted/local sites)\
[East Bay Times](https://www.eastbaytimes.com) -
[Orange County Register](https://www.ocregister.com) -
[St. Paul Pioneer Press](https://www.twincities.com) -
[The Denver Post](https://www.denverpost.com) -
[The Mercury News](https://www.mercurynews.com) -
[The Press-Enterprise](https://www.pe.com)\
*TownNews sites (Blox CMS)* sites (opt-in to custom sites)\
*Tribune Publishing Company* sites like\
[Baltimore Sun](https://www.baltimoresun.com) -
[Capital Gazette](https://www.capitalgazette.com) -
[Chicago Tribune](https://www.chicagotribune.com) -
[Daily Press](https://www.dailypress.com) -
[Hartford Courant](https://www.courant.com) -
[New York Daily News](https://www.nydailynews.com) -
[Orlando Sentinel](https://www.orlandosentinel.com) -
[SunSentinel](https://www.sun-sentinel.com) -
[The Morning Call](https://www.mcall.com) -
[The Virginian-Pilot](https://www.pilotonline.com)

#### Canada
[iPolitics](https://www.ipolitics.ca) -
[Le Devoir](https://www.ledevoir.com) -
[The Globe and Mail](https://www.theglobeandmail.com) -
[The Hill Times](https://www.hilltimes.com) -
[Winnipeg Free Press](https://www.winnipegfreepress.com)

Grouped in options:\
*Postmedia Network* sites like (opt-in to custom sites for unlisted)\
[Calgary Herald](https://calgaryherald.com) -
[Financial Post](https://www.financialpost.com) -
[National Post](https://www.nationalpost.com) -
[The Province](https://theprovince.com) -
[Toronto Sun](https://torontosun.com) -
[Vancouver Sun](https://vancouversun.com)\
*TorStar* sites like\
[The Toronto Star](https://www.thestar.com) and regional sites 
[Niagara Falls Review](https://www.niagarafallsreview.ca) -
[Peterborough Examiner](https://www.thepeterboroughexaminer.com) -
[St. Catharines Standard](https://www.stcatharinesstandard.ca) -
[The Hamilton Spectator](https://www.thespec.com) -
[Waterloo Region Record](https://www.therecord.com) -
[Welland Tribune](https://www.wellandtribune.ca)

#### Europe

[EUobserver](https://euobserver.com)

##### United Kingdom/Ireland
[Belfast Telegraph](https://www.belfasttelegraph.co.uk) -
[Financial News](https://www.fnlondon.com) -
[Financial Times](https://www.ft.com) -
[Investors' Chronicle](https://www.investorschronicle.co.uk) -
[Irish Independent](https://www.independent.ie) -
[London Review of Books](https://www.lrb.co.uk) -
[New Left Review](https://newleftreview.org) -
[Prospect Magazine](https://www.prospectmagazine.co.uk) -
[The Athletic UK](https://theathletic.co.uk) -
[The Economist](https://www.economist.com) -
[The Independent](https://www.independent.co.uk) -
[The New Statesman](https://www.newstatesman.com) -
[The Spectator](https://www.spectator.co.uk) -
[The Telegraph](https://www.telegraph.co.uk) -
[The Times (link to archive.today)](https://www.thetimes.co.uk) -
[The Times Literary Supplement](https://www.the-tls.co.uk) -
[UnHerd](https://unherd.com)

##### Denmark

[Berlingske](https://www.berlingske.dk)

##### Finland
Grouped in options:\
*Sanoma Media Finland* sites like (opt-in to custom sites for unlisted/regional sites)\
[Aamulehti](https://www.aamulehti.fi) -
[Helsingin Sanomat](https://www.hs.fi)

*Alma Talent* sites like\
[Arvopaperi](https://www.arvopaperi.fi) -
[Iltalehti](https://www.iltalehti.fi) -
[Kauppalehti](https://www.kauppalehti.fi) -
[Markkinointi & Mainonta](https://www.marmai.fi) -
[Mediuutiset](https://www.mediuutiset.fi) -
[Mikrobitti](https://www.mikrobitti.fi) -
[Talousel??m??](https://www.talouselama.fi) -
[Tekniikka & Talous](https://www.tekniikkatalous.fi) -
[Tivi](https://www.tivi.fi) -
[Uusi Suomi](https://www.uusisuomi.fi)

##### France/Wallonia
[Alternatives Economiques](https://www.alternatives-economiques.fr) -
[Atlantico](https://atlantico.fr) -
[Causeur](https://www.causeur.fr) -
[Challenges](https://www.challenges.fr) -
[Charlie Hebdo](https://charliehebdo.fr) -
[Connaissance des Arts](https://www.connaissancedesarts.com) -
[Elle](https://www.elle.fr) -
[Esprit](https://esprit.presse.fr) -
[Franc-Tireur](https://www.franc-tireur.fr) -
[L'??cho](https://lecho.be) -
[L'??quipe](https://www.lequipe.fr) -
[L'Express](https://www.lexpress.fr) -
[L'Obs](https://www.nouvelobs.com) -
[L'Oeil de la Photographie (fr/en)](https://loeildelaphotographie.com) -
[L'Opinion](https://www.lopinion.fr) -
[L'Usine Nouvelle](https://www.usinenouvelle.com) -
[La Croix](https://www.la-croix.com) -
[La Libre](https://www.lalibre.be) -
[La Montagne](https://www.lamontagne.fr) -
[La Nouvelle R??publique du Centre-Ouest](https://www.lanouvellerepublique.fr) -
[La Tribune](https://www.latribune.fr) -
[Le Journal du Dimanche](https://lejdd.fr) -
[Le Journal du Net](https://www.journaldunet.com) -
[Le Nouvel Economiste](https://www.lenouveleconomiste.fr) -
[Le Parisien](https://www.leparisien.fr) -
[Le T??l??gramme](https://www.letelegramme.fr) -
[Le Vif](https://www.levif.be) -
[Les ??chos](https://www.lesechos.fr) -
[Les Inrockuptibles](https://www.lesinrocks.com) -
[Marianne](https://www.marianne.net) -
[Paris Match](https://www.parismatch.com) -
[Science & Vie](https://www.science-et-vie.com) -
[Sciences et Avenir](https://www.sciencesetavenir.fr) -
[T??l??rama](https://www.telerama.fr) -
[Valeurs Actuelles](https://www.valeursactuelles.com)

Grouped in options:\
*Groupe EBRA* sites like\
[Derni??res Nouvelles d'Alsace](https://www.dna.fr) -
[L'Alsace](https://www.lalsace.fr) -
[L'Est R??publicain](https://www.estrepublicain.fr) -
[Le Bien Public](https://www.bienpublic.com) -
[Le Dauphin?? Lib??r??](https://www.ledauphine.com) -
[Le Journal de Sa??ne-et-Loire](https://www.lejsl.com) -
[Le Progr??s](https://www.leprogres.fr) -
[Le R??publicain Lorrain](https://www.republicain-lorrain.fr) -
[Vosges Matin](https://www.vosgesmatin.fr)\
*Groupe La D??p??che* sites like\
[Centre Presse](https://www.centrepresseaveyron.fr) -
[L'Ind??pendant](https://www.lindependant.fr) -
[La D??p??che du Midi](https://www.ladepeche.fr) -
[La Nouvelle R??publique des Pyr??n??es](https://www.nrpyrenees.fr) -
[Le Petit Bleu d'Agen](https://www.petitbleu.fr) -
[Midi Libre](https://www.midilibre.fr) -
[Midi Olympique](https://www.midi-olympique.fr)\
*Groupe Nice-Matin* sites like\
[Monaco-Matin](https://www.monacomatin.mc) -
[Nice-Matin](https://www.nicematin.com) -
[Var-Matin](https://www.varmatin.com)\
*Groupe Rossel* sites like\
[L'Aisne nouvelle](https://www.aisnenouvelle.fr) -
[L'Ardennais](https://www.lardennais.fr) -
[L'Est-??clair](https://www.lest-eclair.fr) -
[L'Union](https://www.lunion.fr) -
[La Voix du Nord](https://www.lavoixdunord.fr) -
[Le Courrier picard](https://www.courrier-picard.fr) -
[Le Soir](https://www.lesoir.be) -
[Lib??ration Champagne](https://www.liberation-champagne.fr) -
[Nord ??clair](https://www.nordeclair.fr) -
[Nord Littoral](https://www.nordlittoral.fr) -
[Paris Normandie](https://www.paris-normandie.fr) -
[SudInfo](https://www.sudinfo.be)\
*Groupe Sud Ouest* sites like\
[Charente libre](https://www.charentelibre.fr) -
[La R??publique des Pyr??n??es](https://www.larepubliquedespyrenees.fr) -
[Sud Ouest](https://www.sudouest.fr)

##### Germany/Austria
[Allg??uer Zeitung](https://www.allgaeuer-zeitung.de) -
[Augsburger Allgemeine](https://www.augsburger-allgemeine.de) -
[Automobilwoche](https://www.automobilwoche.de) -
[Badische Neueste Nachrichten](https://www.bnn.de) -
[Berliner Zeitung](https://www.berliner-zeitung.de) -
[Cicero](https://www.cicero.de) -
[Deutsche Wirtschafts Nachrichten](https://deutsche-wirtschafts-nachrichten.de) -
[Die Rheinpfalz](https://www.rheinpfalz.de) -
[Die Zeit](https://www.zeit.de) -
[Frankfurter Allgemeine Zeitung](https://www.faz.net) -
[Freie Presse](https://www.freiepresse.de) -
[Handelsblatt](https://www.handelsblatt.com)* -
[K??lner Stadt-Anzeiger](https://www.ksta.de) -
[K??lnische Rundschau](https://www.rundschau-online.de) -
[Krautreporter.de](https://krautreporter.de) -
[Kurier.at](https://kurier.at) -
[Mitteldeutsche Zeitung](https://www.mz.de) -
[M??nstersche Zeitung](https://www.muensterschezeitung.de) -
[Neue Osnabr??cker Zeitung](https://www.noz.de) -
[Nordwest Zeitung](https://www.nwzonline.de) -
[N??rnberger Nachrichten](https://www.nn.de) -
[Piqd.de](https://www.piqd.de) -
[Rhein-Zeitung](https://www.rhein-zeitung.de) -
[Schleswig-Holsteinischer Zeitungsverlag](https://www.shz.de) -
[Schweriner Volkszeitung](https://www.svz.de) -
[Volksstimme](https://www.volksstimme.de) -
[Westdeutsche Zeitung](https://www.wz.de) -
[Westfalen-Blatt](https://www.westfalen-blatt.de) -
[Westf??lische Nachrichten](https://www.wn.de)

Grouped in options:\
*Funke Mediengruppe* sites like (opt-in to custom sites for unlisted)\
[Berliner Morgenpost](https://www.morgenpost.de) -
[Braunschweiger Zeitung](https://www.braunschweiger-zeitung.de) -
[Hamburger Abendblatt](https://www.abendblatt.de) -
[Neue Ruhr Zeitung](https://www.nrz.de) -
[Ostth??ringer Zeitung](https://www.otz.de) -
[Th??ringer Allgemeine](https://www.thueringer-allgemeine.de) -
[Th??ringische Landeszeitung](https://www.tlz.de) -
[Westdeutsche Allgemeine Zeitung](https://www.waz.de) -
[Westfalenpost](https://www.wp.de) -
[Westf??lische Rundschau](https://www.wr.de)\
*Madsack Mediengruppe* sites like (opt-in to custom sites for unlisted)\
[Hannoversche Allgemeine Zeitung](https://www.haz.de) -
[Kieler Nachrichten](https://www.kn-online.de) -
[Leipziger Volkszeitung](https://www.lvz.de) -
[L??becker Nachrichten](https://www.ln-online.de) -
[M??rkische Allgemeine](https://www.maz-online.de) -
[Neue Presse (Hannover)](https://www.neuepresse.de) -
[Ostsee-Zeitung](https://www.ostsee-zeitung.de) -
[RedaktionsNetzwerk Deutschland](https://www.rnd.de)

##### Italy
[Corriere della Sera](https://www.corriere.it) -
[Domani](https://editorialedomani.it) -
[Eastwest](https://eastwest.eu) -
[GElocal.it](https://quotidiani.gelocal.it) -
[Huffingtonpost.it](https://www.huffingtonpost.it) -
[Il Fatto Quotidiano](https://www.ilfattoquotidiano.it) -
[Il Foglio](https://www.ilfoglio.it) -
[Il Secolo XIX](https://www.ilsecoloxix.it) -
[Internazionale](https://www.internazionale.it) -
[Italia Oggi](https://www.italiaoggi.it) -
[Italian.tech](https://www.italian.tech) -
[La Nuova Sardegna](https://www.lanuovasardegna.it) -
[La Repubblica](https://www.repubblica.it) -
[La Stampa](https://www.lastampa.it) -
[Le Scienze](https://www.lescienze.it) -
[LimesOnline (it/en)](https://www.limesonline.com)

Grouped in options:\
[Il Messaggero](https://www.ilmessaggero.it) and regional sites like
[Corriere Adriatico](https://www.corriereadriatico.it) -
[Il Gazzettino](https://www.ilgazzettino.it) -
[Il Mattino](https://www.ilmattino.it) -
[Quotidiano di Puglia](https://www.quotidianodipuglia.it)\
[Quotidiano Nazionale](https://www.quotidiano.net) and regional sites like
[Il Giorno](https://www.ilgiorno.it) -
[Il Resto del Carlino](https://www.ilrestodelcarlino.it) -
[Il Telegrafo Livorno](https://www.iltelegrafolivorno.it) -
[La Nazione](https://www.lanazione.it)

##### Netherlands/Flanders
[De Morgen](https://www.demorgen.be) -
[De Tijd](https://www.tijd.be) -
[Financieele Dagblad](https://fd.nl) -
[Follow the Money](https://www.ftm.nl) -
[Groene Amsterdammer](https://www.groene.nl) -
[Humo](https://www.humo.be) -
[Knack](https://www.knack.be) -
[NRC Handelsblad](https://www.nrc.nl) -
[Parool](https://www.parool.nl) -
[Telegraaf](https://www.telegraaf.nl) -
[Trouw](https://www.trouw.nl) -
[Volkskrant](https://www.volkskrant.nl) -
[Vrij Nederland](https://www.nl.nl)

Grouped in options:\
*Mediahuis Nederland Regional* sites like\
[Noordhollands Dagblad](https://www.noordhollandsdagblad.nl) -
[Haarlems Dagblad](https://www.haarlemsdagblad.nl) -
[Leidsch Dagblad](https://www.leidschdagblad.nl) -
[IJmuider Courant](https://www.ijmuidercourant.nl) -
[De Gooi- en Eemlander](https://www.gooieneemlander.nl)\
*Mediahuis Noord* sites like (opt-in to custom sites for unlisted):\
[Dagblad van het Noorden](https://www.dvhn.nl) -
[Leeuwarder Courant](https://www.lc.nl)

##### Portugal
[Correio da Manh??](https://www.cmjornal.pt) -
[Observador](https://observador.pt)

##### Slovenia
[Finance.si](https://www.finance.si)

##### Spain
[ABC](https://www.abc.es) -
[El Confidencial](https://www.elconfidencial.com) -
[El Diario.es](https://www.eldiario.es) -
[El Espa??ol](https://www.elespanol.com) -
[El Mundo](https://www.elmundo.es) -
[El Pa??s](https://elpais.com) -
[El Peri??dico de Catalunya](https://www.elperiodico.com) -
[Expansi??n](https://www.expansion.com) -
[La Vanguardia](https://www.lavanguardia.com) -
[Marca](https://www.marca.com) -
[Pol??tica Exterior](https://www.politicaexterior.com)

Grouped in options:\
*Grupo Prensa Ib??rica* sites like (opt-in to custom sites for unlisted):\
[Diario de Mallorca](https://www.diariodemallorca.es) -
[El D??a](https://www.eldia.es) -
[El Peri??dico de Espa??a](https://www.epe.es) -
[Faro de Vigo](https://www.farodevigo.es) -
[Informaci??n](https://www.informacion.es) -
[La Nueva Espa??a](https://www.lne.es) -
[La Provincia](https://www.laprovincia.es) -
[Levante-EMV](https://www.levante-emv.com)\
*Grupo Vocento* (ABC regional) sites like\
[Diario Vasco](https://www.diariovasco.com) -
[El Comercio](https://www.elcomercio.es) -
[El Correo](https://www.elcorreo.com) -
[El Diario Monta????s](https://www.eldiariomontanes.es) -
[El Norte de Castilla](https://www.elnortedecastilla.es) -
[Hoy](https://www.hoy.es) -
[Ideal](https://www.ideal.es) -
[La Rioja](https://www.larioja.com) -
[La Verdad](https://www.laverdad.es) -
[La Voz de C??diz](https://www.lavozdigital.es) -
[Las Provincias](https://www.lasprovincias.es) -
[Sur](https://www.diariosur.es)

##### Sweden
[Aftonbladet](https://www.aftonbladet.se) -
[Dagens Industri](https://www.di.se) -
[Dagens Nyheter](https://www.dn.se)* -
[NyTeknik](https://www.nyteknik.se)

##### Switzerland
[Neue Z??rcher Zeitung (+ regional/opt-in to custom sites)](https://www.nzz.ch) -
[The Market](https://themarket.ch)

#### Africa

###### Kenya

[Daily Nation](https://nation.africa)

#### Australia/New Zealand

[Brisbane Times](https://www.brisbanetimes.com.au) -
[Eureka Report](https://www.eurekareport.com.au) -
[Griffith Review](https://www.griffithreview.com) -
[Intelligent Investor](https://www.intelligentinvestor.com.au) -
[New Zealand Herald](https://www.nzherald.co.nz) -
[The Age](https://www.theage.com.au) -
[The Australian Financial Review](https://www.afr.com) -
[The Saturday Paper](https://www.thesaturdaypaper.com.au) -
[The Spectator Australia](https://www.spectator.com.au) -
[The Sydney Morning Herald](https://www.smh.com.au) -
[The West Australian (+ regional/opt-in to custom sites)](https://thewest.com.au) -
[WAtoday](https://www.watoday.com.au)

Grouped in options:\
*News Corp Australia* site like\
[Cairns Post](https://www.cairnspost.com.au) -
[Code Sports](https://www.codesports.com.au) -
[Geelong Advertiser](https://www.geelongadvertiser.com.au) -
[Gold Coast Bulletin](https://www.goldcoastbulletin.com.au) -
[Herald Sun](https://www.heraldsun.com.au) -
[Northern Territory News](https://www.ntnews.com.au) -
[The Advertiser/AdelaideNow](https://www.adelaidenow.com.au) -
[The Australian](https://www.theaustralian.com.au) -
[The Chronicle](https://www.thechronicle.com.au) -
[The Courier-Mail](https://www.couriermail.com.au) -
[The Daily Telegraph](https://www.dailytelegraph.com.au) -
[The Mercury Tasmania](https://www.themercury.com.au) -
[The Weekly Times](https://www.weeklytimesnow.com.au) -
[Townsville Bulletin](https://www.townsvillebulletin.com.au)\
*Australian Community Media (daily)* sites like (opt-in to custom sites for unlisted)\
[Bendigo Advertiser](https://www.bendigoadvertiser.com.au) -
[Central Western Daily](https://www.centralwesterndaily.com.au) -
[Daily Liberal](https://www.dailyliberal.com.au) -
[Illawarra Mercury](https://www.illawarramercury.com.au) -
[Newcastle Herald](https://www.newcastleherald.com.au) -
[The Advocate](https://www.theadvocate.com.au) -
[The Border Mail](https://www.bordermail.com.au) -
[The Canberra Times](https://www.canberratimes.com.au) -
[The Courier](https://www.thecourier.com.au) -
[The Daily Advertiser](https://www.dailyadvertiser.com.au) -
[The Examiner](https://www.examiner.com.au) -
[The Northern Daily Leader](https://www.northerndailyleader.com.au) -
[The Standard](https://www.standard.net.au) -
[Western Advocate](https://www.westernadvocate.com.au)

#### East Asia
[Asia Times](https://asiatimes.com) -
[CommonWealth Magazine Taiwan](https://www.cw.com.tw)* -
[Harvard Business Review China](https://www.hbrchina.org) -
[Mainichi Shimbun](https://mainichi.jp) -
[Nikkei Asian Review](https://asia.nikkei.com) -
[South China Morning Post](https://www.scmp.com) -
[Southern Weekly](https://www.infzm.com) -
[Tech in Asia](https://www.techinasia.com) -
[The Diplomat](https://thediplomat.com) -
[The Star Malaysia](https://www.thestar.com.my)

#### India
[Bloomberg Quint](https://www.bloombergquint.com) -
[Business Standard](https://www.business-standard.com) -
[Hindustan Times](https://www.hindustantimes.com) -
[Inc42](https://inc42.com) -
[India Today](https://www.indiatoday.in) -
[Live Law](https://www.livelaw.in) -
[LiveMint](https://www.livemint.com) -
[MediaNama](https://www.medianama.com) -
[Mid-Day](https://www.mid-day.com) -
[Outlook](https://www.outlookindia.com) -
[The Economic Times (ET Prime)](https://economictimes.indiatimes.com) -
[The Hindu](https://www.thehindu.com) -
[The Hindu BusinessLine](https://www.thehindubusinessline.com) -
[The Indian Express](https://indianexpress.com) -
[Times of India](https://timesofindia.indiatimes.com)

#### Israel
[Globes](https://www.globes.co.il) -
[Haaretz.co.il](https://www.haaretz.co.il) -
[Haaretz.com](https://www.haaretz.com) -
[The Jerusalem Post](https://www.jpost.com) -
[The Marker](https://www.themarker.com)

#### Latin America

##### Argentina
[??mbito](https://www.ambito.com) -
[Clar??n](https://www.clarin.com) -
[La Naci??n](https://www.lanacion.com.ar)
##### Brazil
[Exame](https://exame.com) -
[Folha de S. Paulo](https://www.folha.uol.com.br) -
[Grupo Abril](https://grupoabril.com.br) -
[O Estado de S. Paulo](https://estadao.com.br) -
[O Globo](https://oglobo.globo.com) -
[Valor Econ??mico](https://valor.globo.com)*
##### Chile
[Diario Financiero](https://www.df.cl) -
[El Mercurio](https://digital.elmercurio.com) -
[El Mercurio de Valpara??so](https://www.mercuriovalpo.cl) -
[La Estrella de Valpara??so](https://www.estrellavalpo.cl) -
[La Segunda](https://digital.lasegunda.com) -
[La Tercera](https://www.latercera.com)
##### Colombia
[El Espectador](https://www.elespectador.com) -
[El Tiempo](https://www.eltiempo.com)
##### Mexico
[Mexico News Daily](https://mexiconewsdaily.com)
##### Peru
*Grupo El Comercio* sites like:
[Diario Correo](https://diariocorreo.pe) -
[El Comercio](https://elcomercio.pe) -
[Gesti??n](https://gestion.pe)

_* free/cached articles only._

### Sites with limited number of free articles
The free article limit can normally be bypassed by removing cookies for the site.  
Click on the BPC-icon and then 'clear cookies'-button in the popup (for unsupported sites grant permission for domain).  
If removing the cookies works you can also add the site as a custom site.

### New site requests
You can [submit a request for a new website](https://gitlab.com/magnolia1234/bypass-paywalls-firefox-clean/-/issues).  
Please read the following instructions and share your results for a quicker process.  
Remember to check the [previous requests](https://gitlab.com/magnolia1234/bypass-paywalls-firefox-clean/-/issues?scope=all&state=all) before asking for a new website.  
1. Open incognito window and search for article in Google search (or webcache).
2. Clear cookies for the site (by this add-on: opt-in to custom sites or grant permission for the site; also enables blocking of general paywall scripts).
3. Disable Javascript on the site (by browser, uBlock Origin or other add-on).
4. Add the domain as custom site for more bypass options.
5. Open page in reader view (by browser or add-on).

### Add custom site
Add your own custom site (also for testing).  
Check 'Options'-link in popup-menu and go to custom sites.
\* by default BPC has limited permissions, but you can opt-in to enable custom sites (and also clear cookies/block general paywall-scripts for non-listed sites). You can also just request permissions for the custom sites you added yourself (or `clear cookies` (BPC-icon) to ask for permission for current site).

By default sites' cookies/local storage are removed after page loads (to bypass article limit).  
Also you can enable Googlebot/Bingbot user-agent, set referer (to Facebook, Google or Twitter; ignored when Googlebot is set), set random ip-address, disable Javascript for (sub)domain(s) and/or external domains, block regular expression, unhide text on (or when paywall(selector) redirect to) amp-page and/or load text from json (paywall|article selector).

[Example list of custom sites](https://gitlab.com/magnolia1234/bypass-paywalls-firefox-clean/-/blob/master/custom/sites_custom.json) or [download list (json)](https://gitlab.com/magnolia1234/bypass-paywalls-firefox-clean/-/raw/master/custom/sites_custom.json)

PS on Android: enabling custom sites isn't working (no optional permissions).\
Then you need the 'custom' add-on version (with access to all sites): [Bypass Paywalls Clean (custom)](https://addons.mozilla.org/en-US/firefox/addon/bypass-paywalls-clean-custom)

### Add excluded site
Add excluded sites/domains (for your subscriptions).\
You can also exclude a specific domain which is grouped in options.

### Troubleshooting
* This add-on works best alongside the adblocker [uBlock Origin](https://addons.mozilla.org/en-US/firefox/addon/ublock-origin).
* Add usefull custom filter [Fanboy's Enhanced Tracking List](https://www.fanboy.co.nz/enhancedstats.txt)
* If a site doesn't work, try turning off uBlock and refreshing.
* Make sure the (new) site is checked under Options.
* You will be logged out for most of the sites you have checked.
* Make sure you're running the latest version of Bypass Paywalls Clean.
* If none of these work, you can [submit an issue](https://gitlab.com/magnolia1234/bypass-paywalls-firefox-clean/-/issues).
* If you live in the EU, also consider installing the extension [I don't care about cookies](https://addons.mozilla.org/en-US/firefox/addon/i-dont-care-about-cookies) in order to remove cookie warnings (or add filter [Easylist Cookies](https://easylist-downloads.adblockplus.org/easylist-cookie.txt) | [I don't care about cookies custom filter](https://www.i-dont-care-about-cookies.eu/abp) to uBlock Origin). Some sites need to set a consent-cookie for (social) media.

### Changelog-releases
* Visit the [changelog page](https://gitlab.com/magnolia1234/bypass-paywalls-firefox-clean/-/blob/master/changelog.txt).
* Or check the [commits](https://gitlab.com/magnolia1234/bypass-paywalls-firefox-clean/-/commits/master).
* [Download the latest version](https://gitlab.com/magnolia1234/bypass-paywalls-firefox-clean/-/releases)

### License
Bypass Paywalls Clean is [MIT-licensed](https://gitlab.com/magnolia1234/bypass-paywalls-firefox-clean/-/blob/master/LICENSE).

### Disclaimer
* This software is provided for educational purposes only and is provided "AS IS", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose and noninfringement. In no event shall the authors or copyright holders be liable for any claim, damages or other liability, whether in an action of contract, tort or otherwise, arising from, out of or in connection with the software or the use or other dealings in the software.
