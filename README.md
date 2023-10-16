# soldier
Self Sustained Uber, Ola, or Lyft
// SPDX-License-Identifier: MI
pragma solidity ^0.6.0;

contract SevenInputContract {
    // State variables to store the inputs and the result
    uint256 public ride_request;
    uint256 public odour;
    uint256 public bin;
    uint256 public residue;
    uint256 public mileage;
    uint256 public petrol;
    uint256 public payment;

    constructor() {
        // Initialize the state variables with default values
        ride_request = 0;
        odour = 0;
        bin = 0;
        residue = 0;
        mileage = 0;
        petrol = 0;
        payment = 0;
    }

    // Function to set the 7 inputs
    function setInputs(uint256 _input1, uint256 _input2, uint256 _input3, uint256 _input4, uint256 _input5, uint256 _input6, uint256 _input7) public {
        request = _request;
        odour = _odour;
        bin = _bin;
        residue = _residue;
        mileage = _mileage;
        payment = _payemnt;
    }

    // The following numbers are just examples for what the value might be for the different inputs given by the car.
    function performCalculation() public {   // This is to accept the erquest if it is nearby
        if (request ==1) {
            result = ("check availability to accept")
            _payemnt=1  // Whenever the rider leave the ride, the payment will be deducted from his wallet and added to the blockchain of the car. 
            }
            
        if (odour>100) {                    // This is to check if the car's odour is acceptable by the rider. That is, it will check for a general odour. 
            result = ("goes for cleaning")
            }
            
        if (bin=100) {                      // Whenever a rider exits the car, the car's vaccum will activate and deposit any waste in the bins located on the sides. When the bin is full, it will dump the trash.
            result = ("dumps the trash in a dumpster")
            }
            
        if (residue>100) {   // This is to see if the engine is working effeciently. Whenever the engine needs maintainence, its emits carbon particles. This will take the car for servicing if needed.
            result = ("goes for pollution check")
            }
            
        if (mileage<100) {   //If the car's average decrease more than a set limit, the car will be considered not okay for the rides and discarded, ensuring the enviornment.
            result = ("the car is no longer good for the drive. Discarded")
            }
    }
}
