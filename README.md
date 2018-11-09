# A Standard for Responsible Disclosure in Cryptocurrency and Related Software
This is a fork of Responsible Disclosure document outlined here: https://github.com/RD-Crypto-Spec/Responsible-Disclosure

bcoin intends to follow this specification. An addedum with details specific to the project, such as contact info & bounty details, can be found at the end of this document.

## Background
Cryptocurrencies represent a radical shift from the legacy financial system and as a result provide an opportunity to help reshape the finance world. It is essential to recall that cryptocurrencies represent real money and introducing bugs and security vulnerabilities can cost users a significant amount of money, but ultimately hurt all other participants in the space.

There are several open source projects with common code, with shared goals of expansion in capability and investment, driven by market confidence in their integrity, that would benefit from a safe and well-defined vulnerability sharing processes.

For this reason, we have formalized a Responsible Disclosure policy that sets a standard for how organizations can share vulnerability information ethically, responsibly and for the good of the ecosystem.

## Guiding Principles
- We recognize that prior to mainstream adoption of cryptocurrencies, the safety and associated growth of the ecosystem of technologies is more important than competition within the space, at least when considering security vulnerability information.
- We recognize that universal adoption of basic security responses to disclosures is vital to the prosperity of the ecosystem and by extension every member of it.
- We recognize that this standard must reflect and respect the complexities of the crypto ecosystem and provide the opportunity for organizations to adhere to their own values and working practices beyond this basic standard.

## Purpose
This standard is intended to set the expectations and limitations of the disclosure process and each party’s participation in it, to reduce the effort and confusion involved in disclosing vulnerabilities, and to encourage participation in vital security practices for the benefit of all participants.

## The Standard
To adhere to this standard, your organization will need to publish a document describing your disclosure process and follow the basic practices involved. This document is a suggested starting point. Publishing can be achieved using GitHub, but wherever it is published it should be possible to link directly to it with a static url so that it can be linked by other participating organizations. 

### Ethical Behavior
Responsible disclosure is predicated on ethical behavior. These guidelines outline best practices for the community as whole, whether you are reporting, or the recipient of a report. By stating that you adhere to this policy, you’re claiming to handle vulnerability information ethically, and abide by the following:

- Do not attempt to leverage a vulnerability, or information of its existence, as part of a financial trading strategy.
- Do not attempt to compromise systems upon which development of a product relies; including but not limited to compromising development systems, accounts, domains, email etc..
- Do not attempt to sell vulnerabilities.
- Do not ask for any form of compensation from an affected party.
- You may compensate a disclosing party if you would like to after all known vulnerability details have been disclosed.
- Do not disclose a bug or vulnerability on mailing lists, public boards, forums, social media or any other channel prior to Responsibly Disclosing to the organizations you have a published relationship with
- Do not attempt any illegal acts, including phishing, physical attacks, DDoS, or any attempt to gain access without authorization

### Publicly Committing to Disclosure Process
To commit to this standard it requires that your published disclosure process include an addendum section that outlines policies specific to your project.

1. Your preferred contact method (eg. email to this address)
2. How to use that contact method securely (eg. full public key)
3. Details of any bug bounty program if you have one, and what it does or does not cover (you can link to another single page that contains these details).
4. Your list of neighboring projects who you will disclose to if you find an issue or if an issue is disclosed to you that might affect their products too.
5. A link to this standard.
6. The date that your commitment was last updated.

### Publicly Committing to Disclosure Relationships
To provide ecosystem cohesion and the expectation of cooperation and timely delivery of vulnerability information, each participating organization will publicly commit to making disclosures that may affect related projects (‘neighbors’). This does not limit any participating organization from responsibly disclosing to other organizations, provided that they follow the other provisions and restrictions of this standard when doing so.

Committing to disclosure relationships serves the purpose of setting the expectation of sharing by proxy to those parties should it be likely they are also affected by a disclosed bug. The intention is that all affected parties will collaborate on fixes, release updates together, then release vulnerability details together in concert with the original disclosing party.

### Standard Disclosure Timelines
Some vulnerabilities take more time to fix than others, and some organizations are able to switch tasks to fixes faster than others, and this ability tends to fluctuate over time.

### Initial Contact
To disclose to a neighbor that you have an existing relationship with, you must contact them via their published contact details using the security procedures that they have published. If you get no response within two working days, you must try another two times with an interval of two working days each time. If you get no acknowledgement to those messages, you may optionally decide to attempt to reach them using other methods, but you must not include details of the vulnerability unless you are using their approved secure communication method.

If there is no response after your initial contact attempts, you should send another message saying that there has been no response to your (at least three) messages and setting a date for public disclosure that is not less than 90 days in the future and not more than sixty days. If you receive a response during that time, both parties can agree to change the disclosure date in accordance with the rest of this process.

### Giving Details
After you receive a response to your initial contact, you should disclose the details of the vulnerability to the potentially affected party, along with reasons you think they may be affected and any advice you have on how to fix the issue.
Once you have made initial contact, you are expected to provide all the technical details about the vulnerability within two working days of receiving acknowledgement of your initial contact.

Your report should include:
- A PGP encrypted email to maintainers
- Description of suspected vulnerability
- Steps to reproduce the issue
- Your email address and a secure mechanism to contact you
- Your name and/or colleagues if you wish to be later recognized
- Optionally a patch and/or suggestions to resolve the vulnerability

### Setting Dates
After you have provided details of the issue to your neighbors, you both should agree on a date to release updates and a date to publicize the details of the issue. Issues that require only a small change should correspond with a date relatively soon after giving details - somewhere between 30 and 60 days. Issues that require a more significant investment by both parties might result in a date set up to 90 days in the future.

Parties involved in the disclosure should have the expectation of negotiating publishing dates with all of their neighbors that share the affected code, even if it turns out that those neighbors are not vulnerable for some other reason not known at the time.

It is up to each organization to determine their level of vulnerability to any disclosed issue, and rate issues accordingly. In general though, spend bugs should be considered very high priority - users losing access to their funds is precisely what this standard is intended to address.

It is up to each organization to notify their users of the availability of a fix and migrate their user base to the fixed version.

### Coordinated Release
When executed faithfully, the intention of this standard is to have all affected parties release a fix for an issue to their users together, and then all release details of the vulnerability together after a period of time that everyone can agree on.

In practice this is not always possible, and sometimes it will be necessary to release when one or more parties are not ready. Without the threat of public release of vulnerability information, organizations aren’t always incentivized to act in good faith for the security of their users.

Once the dates are set, the clock is very much ticking: When the release date comes around, any and all participating parties should release the vulnerability information regardless of the availability of fixes and the adoption rate of their user base.

Responding with appropriate development resources to fix security bugs, implementing a user contact system, and an update system that can perform in this time-limited scenario is down to each participating organization.

At time of release, participants should make a reasonable effort to discreetly patch. Avoid language that can draw undue attention to commits & PRs, or consider embedding the fix among other updates.

### Bounty Payments
Parties that have been disclosed to may, at their discretion, decide to pay a bounty to a disclosing party, but within the limits of their existing relationship (in the case of a neighbor), or their published bug bounty program (in the case of anyone else). Organizations implementing this standard may not attempt to coerce payments or sell bugs (see the section on “Ethical Behavior”). 

### Acknowledgements
If the reporting individual or organization would like to be recognized for their discovery, they may do so after the disclosure timeout. At the discretion of each participating team, a list of these individuals and/or organizations may recognize vulnerabilities disclosed responsibly.

# bcoin addendum
## Acknowledgements
Should you responsibly disclose a bug to the bcoin team, and would like acknowledgement, we'd be happy to accomodate.

## Bounties
bcoin offers no bounty program at this time. check back soon for an update.

## Contact Info
```
Lead Maintainer
jj @ purse . io
-----BEGIN PGP PUBLIC KEY BLOCK-----
Version: GnuPG v2

mQENBFFPEEwBCACt4A3YR0QLEy5Mo40bqluqAbnQ4E3Gp/FG/xXrXra9/2BXxDjW
ZaDXUI86jJXJ5ko5ZrMwb6u7qJZBXoogcgwgqvrhxorpmm7SLRw4VIRHn8E8D+yk
5rJ+CexFREGeScWcu7+zuJ336ag7kFzaWcc9BFUFXooIAzUUVWKLB28DnX+fbt02
eBz2YxPpmdKnE33einvpiQulYejAA2ZdTyXN7Z39jgwWbehv9pwxNclUYtGSvicE
aiCTS/g0x9jZigK3cS7MqfU7SEDOVIM+NHNUje7E1HokY3T0+s3uy9cJwft+QOvK
MjlzzBlV4ncqxH2MVBeeefx4uUFubq3aopFDABEBAAG0KkNocmlzdG9waGVyIEpl
ZmZyZXkgPGNoamplZmZyZXlAZ21haWwuY29tPokBOAQTAQIAIgUCUU8QTAIbAwYL
CQgHAwIGFQgCCQoLBBYCAwECHgECF4AACgkQiWKrneZma73/Uwf/Qb4t67yAvSHb
ZWzoQyFu4tYJLTNRV7kJW09kP+XULnEspgJn8u/Y7AMTt3KylmNizLQwrWxzqMQD
/kv1WkPopYfbztzfOgEPgxSM347ZYyouCLArwlqhJleOzjDkJYy4hwnY7tf3Axbj
uAoaXnmJ/IqIsluzbHtN9pjdioEGoWQkS+V39fzC0cGZpCoypbcgPM7HKrlR41Ok
MDfApGu2IdmRa9zj09bfPwcYOR1wTxL0VzdbOTUAxHKfdlhYmdj/FZrPJGbhGelQ
gk/PrZkBsyMrtuJ2nmJDGsLe4MP+ufijzowN4R25Dw01vYjWjfEPe/oRElmizuzA
LZcPKuTHErkBDQRRTxBMAQgA/KcvlYqRehiEMq3HyOmaZrVT0NK1uTg9bFVj6srQ
DpnR77uL4i2GLF+Nmu9Wg3L1zrOjwOBNAZ/OSCLnFkrsG2QYjgdSvpHOrPVkoLqh
8XtzFLVhnpz79Q6UChDNvTSs4hemfb2GCloDF+CulU8I98KK1+En6KJ8ppwGdno5
bhHhs09irdxrJUGblS63jKqirFkH0P9BEpjNnroVPUtqV1Dr57ik9XkSD6wR82SW
VlWgJvzO1bS/GnymakbtCx+VfdnB7Nx44bgnqgjtK1/vD7Dl2xacTiem7G/8+Zr+
/MBVANL+RlzhKtIZ5dGn+NkZff2otF6OBGVHgCuXzSOgTwARAQABiQEfBBgBAgAJ
BQJRTxBMAhsMAAoJEIliq53mZmu9XmcIAKAEofa7v+b8nHH+lDMuPMi9jFtrLTwf
JE4KkcTrDPdDdKOgUCjB3nELgXY4ghPo1564ACAMiZrzBOdxFIcLI8NPwj2Ifn0L
E6f82ea+sMcuRDRRz/jGq7oK5x9br+Q6QMWnbjcBEOtkRtrz5dcxVOytY/CC/JJ3
ZBjg9Fq6DsC6bk+8DknY9H1HG7O0OAmifeklePCGXE2BifO0TGsK4/yVvUQ6GhXw
sbHgKZvRKuGZc7i0yTIJnXjg3O63yy08dJYxDBNCAiufFLgv/BxB6hRb1mvJAlBP
r+qJzzEj5Q0gZlgwARbCztpFcOi9yNnriJ5FZ6BjXLBrj87cwSq3wzM=
=EUHU
-----END PGP PUBLIC KEY BLOCK-----
```

```
Project Maintainer
Steven Bower
steven @ purse . io

-----BEGIN PGP PUBLIC KEY BLOCK-----
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
=gGZp
-----END PGP PUBLIC KEY BLOCK-----
```


```
Buck Perley
Project Maintainer
bucko @ purse . io

-----BEGIN PGP PUBLIC KEY BLOCK-----
Version: Keybase Go 1.0.44 (darwin)
Comment: https://keybase.io/bucko

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
=058m
-----END PGP PUBLIC KEY BLOCK-----
```

```
Braydon Fuller
Project Maintainer
braydon @ purse . io
-----BEGIN PGP PUBLIC KEY BLOCK-----

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
e7BqfFjOTUZMsAsyzLaJ
=ennq
-----END PGP PUBLIC KEY BLOCK-----
```

Reference links:
https://medium.com/mit-media-lab-digital-currency-initiative/reducing-the-risk-of-catastrophic-cryptocurrency-bugs-dcdd493c7569 
https://medium.com/mit-media-lab-digital-currency-initiative/http-coryfields-com-cash-48a99b85aad4 
https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2017-September/015036.html 
http://bitcoincore.org/en/contact 
https://lists.linuxfoundation.org/pipermail/bitcoin-dev/ 
https://www.reddit.com/r/btc/comments/6zf1qo/peter_todd_
https://www.reddit.com/r/btc/comments/6z827o/chris_jeffrey_
https://www.reddit.com/r/btc/comments/6zb3lp/maxwell_
https://lists.linuxfoundation.org/pipermail/bitcoin-dev/
http://luke.dashjr.org/programs/bitcoin/files/charts/branches.html



