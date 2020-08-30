# amulmilk

pragma solidity 0.4.22 <= 0.6.12;


contract amulmilk{
    string nameofpacket;
    string dateofmanufacture;
    string coustomername;
    string expiry;
    string colorofthepacket;
    int cost;
    
    
    function amulmilk(string newnameofpacket, string newdateofmanufacture, string newcoustomername, string newexpiry, string newcolorofthepacket, int newcost) public{
        nameofpacket = newnameofpacket;
        dateofmanufacture = newdateofmanufacture;
        coustomername = newcoustomername;
        expiry = newexpiry;
        colorofthepacket = newcolorofthepacket;
        cost = newcost;
    }
    
    function getamulmilk() public view returns(string, string, string, string, string, int){
        return(nameofpacket, dateofmanufacture, coustomername, expiry, colorofthepacket, cost);
    }

}
