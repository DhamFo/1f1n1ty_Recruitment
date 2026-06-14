Blind XXE with out-of-band interaction via XML parameter entities:

    -Since this needed to be done in Collaborator options in Burp suite , it only exist in Pro so i cant use it
    -For security reason  noraml entites are blocked so we will use parameter entities %
    -<!DOCTYPE foo [<!ENTITY % xxe "COLLABORATOR"> % xxe;]>