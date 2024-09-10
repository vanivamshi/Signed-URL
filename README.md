# Signed URL Program
Signed URL generator with,
1) Key Rotation and Versioning - The KEY_VERSIONS dictionary stores secret keys associated with different versions. The generate_signed_url function includes the key version in the URL and uses the corresponding secret key to sign it. The verify_signature function checks the signature using the correct secret key based on the version.
2) IP Whitelisting - The ALLOWED_IPS set contains the IP addresses that are permitted to access the resource. The resource route checks the client’s IP address against the allowed list and rejects requests from unauthorized IPs.
