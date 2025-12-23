# base654
Detecting Proxy Contracts via Bytecode
code = w3.eth.get_code(addr).hex()
if "delegatecall" in code:
    print("Likely proxy contract")
