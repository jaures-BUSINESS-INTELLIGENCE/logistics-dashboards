## Reflection 1 — Who will disagree most?

I predict that the strategic/network manager will disagree most with the other two.

The CO2 manager and the cost manager both look at what the existing routes cost today (in CO2 or in euros). If a warehouse sends very little, they will probably say it is not useful, and they may want to close it or change nothing. The network manager looks at something different: how far all the customers are from a warehouse. For this person, opening a new warehouse (for example in Marseille or Bordeaux) or keeping a small one can be a good idea, even if it does not reduce CO2 or cost today.

So I expect the biggest disagreement to be about closing or opening a warehouse. I will check this after Step 10.

<!-- Réflexion 1 — Qui sera le plus en désaccord ?
Je prédis que le responsable stratégie/réseau sera le plus en désaccord avec les deux autres.
Le responsable CO2 et le responsable coûts regardent ce que les routes existantes coûtent aujourd'hui (en CO2 ou en euros). Si un entrepôt envoie très peu, ils diront probablement qu'il n'est pas utile, et voudront peut-être le fermer ou ne rien changer. Le responsable réseau regarde autre chose : la distance entre tous les clients et un entrepôt. Pour lui, ouvrir un nouvel entrepôt (par exemple à Marseille ou à Bordeaux) ou garder un petit entrepôt peut être une bonne idée, même si cela ne réduit pas le CO2 ni le coût aujourd'hui.
Je m'attends donc à ce que le plus grand désaccord porte sur la fermeture ou l'ouverture d'un entrepôt. Je vérifierai cela après l'étape 10. -->
## Reflection 2 — Which assumption would I defend least?

The assumption I would be least comfortable defending is the cost figures (0.12 EUR per tonne-km for transport and 40 EUR per tonne per year for storage).

These two numbers are not researched and have no source. Real transport prices are commercial and change a lot with the vehicle, the load and the contract, so there is no single official figure. A client could ask "where does this number come from?" and I would have no answer. The cost dashboard also leads to a direct money decision (is the problem transport or storage?), so a wrong number here can change the decision.

The CO2 factor is different: 0.10 kg per tonne-km is inside a real range published by French sources (about 0.047 to 0.12), so I can say where it comes from and check it. The population-as-demand proxy (50 tonnes per 1,000 residents) is also an assumption, but it is at least stated clearly, and it affects all three dashboards in the same way.

<!-- Réflexion 2 — Quelle hypothèse défendrais-je le moins bien ?
L'hypothèse que je défendrais le moins bien est celle des coûts (0,12 EUR par tonne-km pour le transport et 40 EUR par tonne et par an pour le stockage).
Ces deux chiffres ne sont pas recherchés et n'ont pas de source. Les vrais prix de transport sont commerciaux et varient beaucoup selon le véhicule, le chargement et le contrat, donc il n'existe pas de chiffre officiel unique. Un client pourrait demander « d'où vient ce chiffre ? » et je n'aurais pas de réponse. Le dashboard des coûts mène aussi à une décision directe sur l'argent (le problème vient-il du transport ou du stockage ?), donc un chiffre faux ici peut changer la décision.
Le facteur CO2 est différent : 0,10 kg par tonne-km est dans une fourchette réelle publiée par des sources françaises (environ 0,047 à 0,12), donc je peux dire d'où il vient et le vérifier. La demande estimée à partir de la population (50 tonnes pour 1 000 habitants) est aussi une hypothèse, mais elle est au moins clairement annoncée, et elle touche les trois dashboards de la même façon. -->
## Reflection 3 — Two KPIs that point to different actions

I compare the CO2 KPI and the network-distance KPI for the same warehouse: Lille.

In the CO2 view, Lille looks useless. It produces 0 kg of CO2 and 0 EUR of transport cost, because every other city is closer to Paris or Lyon, so Lille only delivers to itself. A CO2 manager looking only at this number could say "there is nothing to improve here", or even "this warehouse does nothing".

In the network view, Lille is useful. If I close it, the average distance for the whole network gets worse (from 168.04 km to 174.43 km), because the 233,098 people of Lille must then be served from Paris. A network manager would say "keep Lille".

So the same warehouse gives two different messages: "ignore it" in the CO2 view, and "keep it" in the network view. A route-based KPI cannot see that a warehouse also serves its own local market.

<!-- Réflexion 3 — Deux indicateurs qui mènent à des actions différentes
Je compare l'indicateur CO2 et l'indicateur de distance du réseau pour le même entrepôt : Lille.
Dans la vue CO2, Lille semble inutile. Il produit 0 kg de CO2 et 0 EUR de coût de transport, car toutes les autres villes sont plus proches de Paris ou de Lyon, donc Lille ne livre que sa propre ville. Un responsable CO2 qui ne regarde que ce chiffre pourrait dire « il n'y a rien à améliorer ici », voire « cet entrepôt ne fait rien ».
Dans la vue réseau, Lille est utile. Si je le ferme, la distance moyenne de tout le réseau empire (de 168,04 km à 174,43 km), car les 233 098 habitants de Lille devraient alors être servis depuis Paris. Un responsable réseau dirait « gardez Lille ».
Un même entrepôt donne donc deux messages différents : « ignorez-le » dans la vue CO2, et « gardez-le » dans la vue réseau. Un indicateur basé sur les routes ne voit pas qu'un entrepôt sert aussi son propre marché local. -->
## Reflection 4 — Would I recommend the #1 route as it is?

The #1 route in my top-10 list is Marseille <- Lyon (about 1,212 tonnes of CO2 per year). I would not recommend it to the sustainability manager without checking a few things first.

First, Marseille is #1 mostly because of its large population (873,076 people), not only because of the distance. The distance (277.6 km) is shorter than Toulouse (359.9 km) or Bordeaux (435.8 km). Since demand is estimated from population (50 tonnes per 1,000 residents), the ranking depends on a proxy, not on real shipments. If Marseille's real volume is different, the ranking changes.

Second, the distances are straight-line distances, not real road distances, so the real CO2 can be higher.

Third, almost all the top routes come from Lyon (Marseille, Toulouse, Bordeaux, Strasbourg, Nice, Montpellier). This suggests that the real problem may be the position of the Lyon warehouse for the south of France, not one single route. Consolidating one route would not fix this.

So I would use this list to decide where to look first, and I would check real shipment data before recommending an action.

<!-- Réflexion 4 — Recommanderais-je la route n°1 telle quelle ?
La route n°1 de mon top 10 est Marseille <- Lyon (environ 1 212 tonnes de CO2 par an). Je ne la recommanderais pas au responsable développement durable sans vérifier quelques points.
D'abord, Marseille est n°1 surtout à cause de sa grande population (873 076 habitants), pas seulement à cause de la distance. La distance (277,6 km) est plus courte que celle de Toulouse (359,9 km) ou de Bordeaux (435,8 km). Comme la demande est estimée à partir de la population (50 tonnes pour 1 000 habitants), le classement dépend d'un proxy, pas de vrais envois. Si le vrai volume de Marseille est différent, le classement change.
Ensuite, les distances sont à vol d'oiseau, pas par la route réelle, donc le vrai CO2 peut être plus élevé.
Enfin, presque toutes les routes du haut partent de Lyon (Marseille, Toulouse, Bordeaux, Strasbourg, Nice, Montpellier). Cela suggère que le vrai problème est peut-être la position de l'entrepôt de Lyon pour le sud de la France, et non une seule route. Regrouper une route ne réglerait pas cela.
J'utiliserais donc cette liste pour décider où regarder en premier, et je vérifierais les vrais volumes avant de recommander une action. -->
## Reflection 5 — Which lever would I pull first for the most expensive warehouse?

The warehouse with the highest total cost is Lyon (about 13.48 million EUR per year). I would pull the transport lever first.

At first sight, storage looks bigger: 7.79 million EUR for storage against 5.69 million EUR for transport. But storage is the same 40 EUR per tonne in every warehouse, so the amount only grows with the tonnage. What makes Lyon different is the cost per tonne: 69.21 EUR for Lyon, against 50.91 EUR for Paris and 40 EUR for Lille. This extra cost comes only from transport, because Lyon serves cities that are far away (Marseille, Toulouse, Bordeaux, Strasbourg). So shortening or consolidating Lyon's long routes is the lever that can really change something.

The weakness of this conclusion is that the 40 EUR for storage is an assumption that I invented, not a real figure. If real storage costs were different between warehouses, the answer could change. I also noticed that the "average cost per tonne" shown on the page (53 EUR) is a simple average of the three warehouses, so small Lille counts as much as big Lyon. The weighted figure (total cost divided by total tonnes) is about 60 EUR. The name of the KPI is the same, but the two ways to compute it give two different numbers.

<!-- Réflexion 5 — Quel levier actionner en premier pour l'entrepôt le plus cher ?
L'entrepôt au coût total le plus élevé est Lyon (environ 13,48 millions d'EUR par an). J'actionnerais d'abord le levier du transport.
À première vue, le stockage semble plus gros : 7,79 millions d'EUR de stockage contre 5,69 millions d'EUR de transport. Mais le stockage vaut 40 EUR par tonne dans tous les entrepôts, donc le montant ne dépend que du tonnage. Ce qui rend Lyon différent est le coût par tonne : 69,21 EUR pour Lyon, contre 50,91 EUR pour Paris et 40 EUR pour Lille. Ce surcoût vient uniquement du transport, car Lyon sert des villes lointaines (Marseille, Toulouse, Bordeaux, Strasbourg). Raccourcir ou regrouper les longues routes de Lyon est donc le levier qui peut vraiment changer quelque chose.
La faiblesse de cette conclusion est que les 40 EUR de stockage sont une hypothèse que j'ai inventée, pas un chiffre réel. Si les vrais coûts de stockage étaient différents selon les entrepôts, la réponse pourrait changer. J'ai aussi remarqué que le « coût moyen par tonne » affiché sur la page (53 EUR) est une moyenne simple des trois entrepôts, donc le petit Lille compte autant que le grand Lyon. Le chiffre pondéré (coût total divisé par tonnes totales) est d'environ 60 EUR. Le nom du KPI est le même, mais les deux façons de le calculer donnent deux chiffres différents. -->
