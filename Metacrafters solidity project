// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract DipikaToken {
    //token details
    string public name = "dipika";
    string public symbol= "DPK";
    uint256 public totalSupply =0;

    // Mapping to store balances
    mapping(address => uint256) public balances;


    // Mint function 
    function mint(address _to, uint256 _value) public {
        totalSupply += _value;
        balances[_to] += _value;
    }

    // Burn function 
    function burn(address _to, uint256 _value) public {
        if(balances[_to] >= _value)
        {
          totalSupply -= _value;
          balances[_to] -= _value;
        }
    }
}
