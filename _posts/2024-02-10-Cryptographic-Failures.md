# Cryptograpic Failures

Hi there, today in this blog post we are going to be talking about cryptographic failures. As number 2 on the OWASP Top Ten,
it is no surprise that this is a big problem in the cybersecurity field. With data needing to be protected, the need for cryptography
is bigger than ever. It's also no surprise that users, who avoid best-practice data protection can worsen the problem.

There are three primary categories of cryptographic failures:
- Access control vulnerabilities
- Failed integrity checks
- Loss of availability



  
Cryptographic failures don't always only expose sensitive information, they can also lead to systems being compromised. Here is a
list of security flaws that commonly lead to cryptographic failures:
- Weak Key Generation: Using Insufficiently random or predictable keys can make encryption vulnerable to brute-force attacks.
- Side-Channel Attacks: Attacks that exploit information leaked during the execution of cryptographic operations, such as timing 
                        attacks, power analysis, or electromagnetic radiation analysis.
- Man-In-The-Middle (MITM) Attacks: Intercepting and modifying encrypted communication between two parties by inserting oneself
                                   as an intermediary. This can be facilitated by weak authentication mechanisms or insecure
                                    key exchange protocols.
- Quantum Computing Threats: Theoretical cryptographic algorithms that are secure against classical computers may be vulnerable
  may be vulnerable to attacks from quantum computers, which could potentially break widely used
  encryption schemes like RSA and ECC.




Many more security flaws could lead to cryptographic failures but we would be here all day if I listed most of them.
Some ways that we as cybersecurity professionals can prevent cryptographic failures are listed below (there are many more besides this):
- Classifying data processed, stored, or transmitted by an application. Identify what data is sensitive according to privacy laws,
  regulatory requirements, and business needs.
- Don't store sensitive data unnecessarily. Discard it as soon as possible or use PCI DSS-compliant tokenization or even
  truncation. Data that is not retained cannot be stolen.
- Ensure up-to-date and strong standard algorithms, protocols, and keys are in place; use proper key management.
- Do not use legacy protocols such as FTP and SMTP for transporting sensitive data.
- Initialization vectors must be chosen appropriately for the mode of operation. For many modes, this means using a CSPRNG
  (cryptographically secure pseudo-random number generator). For modes that require a nonce, then the initialization vector
  (IV) does not need a CSPRNG. In all cases, the IV should never be used twice for a fixed key.

Here is a very good video created by [Crashtest Security](https://www.youtube.com/@crashtestsecurity7689) used on the OWASP website,
take a look (click image):

[![Cryptographic Failures Video](https://img.youtube.com/vi/85Ds9wOPESw/0.jpg)](https://www.youtube.com/watch?v=85Ds9wOPESw)



There is a lot more we could talk about regarding cryptographic failures like salting and seeding, but that is for another day.
Have a great day and come back tomorrow for another blog post!

## Refrences for this Blog post:
- https://crashtest-security.com/owasp-cryptographic-failures/
- https://owasp.org/Top10/A02_2021-Cryptographic_Failures/
- https://chat.openai.com/
