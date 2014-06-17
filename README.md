Guide-Fodbold-Experten-Email-Rentention
=========================================
@@ -0,0 +1,53 @@
iBob Email Retention
========================

Denne guide dækker de skridt der skal til for at få integreret Clerks automatiserede email retention på ibob.dk.

Er der nogle spørgsmål kan du altid kontakte Tim på [thj@clerk.io](mailto:thj@clerk.io).



Opsamling af tilmeldinger i checkout
------------------------------------

For at opsamle emails og øvrige informationer på mailkampagnerne skal følgende attributter indsættes på one step checkout siden.



### Navn

Indsæt følgende attribut på inputfeltet for kundens fornavn:

    data-clerk-campaigns="name"

Se evt pkt. 1 på billedet nedenfor.


### Email

Indsæt følgende attribut på inputfeltet for kundens email:

    data-clerk-campaigns="email"

Se evt pkt. 2 på billedet nedenfor.



### Subscribe

Indsæt følgende kode under den nuværende nyhedsbrevs tilmelding.


    <div class="input-box">
        <input type="checkbox" name="clerk-email" id="clerk-mail-checkbox" value="1" checked="checked" data-clerk-campaigns="subscribe">
        <label for="clerck-mail-checkbox">Ja tak, tilmeld mig relevante tilbud relateret til mine ordrer og aktivitet på ibob.dk</label>
    </div>

Se evt pkt. 3 på billedet nedenfor.



Vejledende billede
------------------

![](/images/guide/ibob-mail/checkout.png) 
