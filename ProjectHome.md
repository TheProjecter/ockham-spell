Given a URL that looks like this:

```
  http://spell.ockham.org/?word=origami
```

the spell service will return an XML stream looking like this:

```
  <spell>
      <version>0.1</version>
      <word>origami</word>
      <dictionary>master</dictionary>
      <spellings>
          <spelling>origami</spelling>
          <spelling>origem</spelling>
          <spelling>irrigam</spelling>
          <spelling>obrigam</spelling>
      </spellings>
  </spell>
```

Clients are then expected to read the XML and provide enhanced services to users. A primary example is to suggest alternative queries to searches that return few or no hits.

This service was implemented as a part of National Science Foundation grant (DUE-0333601) called OCKHAM Library Network, Integrating the NSDL into Traditional Library Services.

Eric Lease Morgan (emorgan@nd.edu), February 27, 2007