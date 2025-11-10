# Understanding TLS 1.3 Handshake
TLS 1.3 has streamlined the handshake process, reducing latency while improving security. Unlike TLS 1.2, 1.3 eliminates obsolete cipher suites and supports forward secrecy by default. I analyzed Wireshark captures of TLS 1.3 handshakes to see the protocol in action.

Key observations: the handshake now combines key exchange with authentication, the client’s “Hello” contains supported groups, and session resumption uses PSK (pre-shared keys). This drastically reduces round trips and makes passive eavesdropping nearly impossible.

Understanding these details is vital for securing web servers, custom clients, or when participating in penetration testing exercises.

[TLS 1.3 RFC](https://www.rfc-editor.org/rfc/rfc8446)
