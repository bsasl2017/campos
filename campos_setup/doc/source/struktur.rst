Event, tilmelding, deltagere og kantaktpersoner
===============================================

I forhold til E2014 er der foretaget nogle forbedringer/foenklinger i modellen:
Der er kun behov for en aktivitet (model: event.event) og ikke et s�rskilt "hj�lperarrangementet"
I stedet har vi en markering p� tilmeldingen om det er en hj�lpertilmelding eller gruppetilmeldingen)

Tilmeldingen (model: event.registration) er "betaleren" og kan b�re flere deltagere. Vil v�re en spejdergruppe eller en hj�lper:

.. image:: images/campinfo.png

Deltageren (model: campos.event.participant) kan s� (for jobbere) knyttes til et udvalg (med godkendelse og mail flows - Disse mails skal ogs� lige forfattes)

B�de Tilmelding og Deltager "nedarver" fra Odoo's generelle kontaktperson object (res.partner), som er det der b�rer navn, adresse, telefon , email etc.

S� i tilf�ldet en "single" hj�lper vil der blive oprettet en Tilmeldingsrecord og en Deltagerrecord, der vil nedarve fra den SAMME res.partner