# Austin Vern Songer #

## Data Communications and Networking ##
     Chapter 8

     Robert Morris University 


----------

### R1

What are the differences between message confidentiality and message
integrity? Can you have confidentiality without integrity? Can you have
integrity without confidentiality? Justify your answer.

Confidentiality is the property that the original plaintext message can not be determined
by an attacker who intercepts the ciphertext-encryption of the original plaintext message.
Message integrity is the property that the receiver can detect whether the message sent
(whether encrypted or not) was altered in transit. The two are thus different concepts,
and one can have one without the other. An encrypted message that is altered in transmit
may still be confidential (the attacker can not determine the original plaintext) but will
not have message integrity if the error is undetected. Similarly, a message that is altered
in transit (and detected) could have been sent in plaintext and thus would not be
confidentia

----------

### R2

Internet entities (routers, switches, DNS servers, Web servers, user end systems,
and so on) often need to communicate securely. Give three specific
example pairs of Internet entities that may want secure communication.




----------

### R3

From a service perspective, what is an important difference between a
symmetric-key system and a public-key system?

One important difference between symmetric and public key systems is that in symmetric
key systems both the sender and receiver must know the same (secret) key. In public key
systems, the encryption and decryption keys are distinct. The encryption key is known
by the entire world (including the sender), but the decryption key is known only by the
receiver.


----------

### R4

Suppose that an intruder has an encrypted message as well as the decrypted
version of that message. Can the intruder mount a ciphertext-only attack, a
known-plaintext attack, or a chosen-plaintext attack?

In this case, a known plaintext attack is performed. If, somehow, the message encrypted
by the sender was chosen by the attacker, then this would be a chosen-plaintext attack.


----------

### R9

In what way does a hash provide a better message integrity check than a
checksum (such as the Internet checksum)?

Suppose Bob sends an encrypted document to Alice. To be verifiable, Alice must be able
to convince herself that Bob sent the encrypted document. To be non-forgeable, Alice
must be able to convince herself that only Bob could have sent the encrypted document
(e.g.,, non one else could have guess a key and encrypted/sent the document) To be nonreputiable,
Alice must be able to convince someone else that only Bob could have sent
the document. To illustrate the latter distinction, suppose Bob and Alice share a secret
key, and they are the only ones in the world who know the key. If Alice receives a
document that was encrypted with the key, and knows that she did not encrypt the
document herself, then the document is known to be verifiable and non-forgeable
(assuming a suitably strong encryption system was used). However, Alice can not
convince someone else that Bob must have sent the document, since in fact Alice knew
the key herself and could have encrypted/sent the document.


----------

### R12
What does it mean for a signed document to be verifiable and non-forgeable?





----------

### R13

In what way does the public-key encrypted message hash provide a better
digital signature than the public-key encrypted message?