# ToDecahedron

ToDecahedron is a Burp Suite extension that identifies and highlights tokens or other patterns directly in HTTP requests and responses. It helps security testers quickly recognize authentication or session tokens during traffic analysis.

## Overview

ToDecahedron marks matching tokens inside Burp’s Proxy and HTTP history views using configurable colors and pattern names. It was designed to detect common token formats such as:

- PASETO (Platform-Agnostic Security Tokens)  
- JWT (JSON Web Tokens)  
- LtpaV2  
- SAML assertions  

By default, ToDecahedron includes built-in regex patterns for SAML, PASETO, JWT, and LtpaV2 tokens. These can be modified or extended through the settings interface.

Although its primary goal is to highlight tokens, ToDecahedron can also be used to detect any user-defined pattern in HTTP headers or body content.

## Features

- Built-in regex rules for SAML, PASETO, JWT, and LtpaV2 tokens  
- Custom regex definitions for additional token types or arbitrary patterns  
- User-defined highlight colors for each pattern  
- Automatic marking of matched tokens in Burp Proxy and HTTP history  
- Notes with pattern names added to matching requests or responses  
- General-purpose pattern detection in headers and bodies  

## Configuration

In the ToDecahedron settings panel, you can:

1. Add or edit regex patterns for the tokens or text you want to detect  
2. Assign a custom highlight color to each pattern  
3. Optionally rename the pattern to control the note label attached to matches  

When a match occurs, ToDecahedron highlights it with the configured color and adds a note containing the pattern’s name to the corresponding request or response. This makes it easy to follow where tokens appear and group them by type.

## Use Cases

- Highlight PASETO, JWT, LTCAV2, or SAML tokens for quick identification  
- Detect and label session identifiers in authentication flows  
- Visually tag sensitive elements such as API keys or secrets  
- Extend detection with custom regex patterns for proprietary tokens  

## License

This project is released under the GPL License.
