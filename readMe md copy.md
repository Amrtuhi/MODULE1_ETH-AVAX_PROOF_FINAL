# Project Title
Error Handling and its methods

This is the Module 1 assesment of Eth+AVAX proof course . This is a solidity program for implementing the error handling concept and its method which consist of require() revert() and assert() methods  .

## Description

This is a program which is created in solidity for using the concept of errror handling and implementing its methods which uses the basic concept of solidity like working in remix ethereum and writing a code in .sol file which contains the intermediate knowledge like error handling and its methods . This program show the use of error handling methods and also its implementation.

## Getting Started


### Executing program

To run this program , i am using Remix , an Solidity IDE.
->To start go to Remix IDE and start coding 
->add a solidity file i named it as odd_even.sol
->include the licence (SPDX) 
->use the latest solidity compiler by including the pragma which will compiler the code using that solidity compiler.
->make a contract named odd_even
->under that contract create three function named requireOddNumber which take one parameters of unsigned interger (uint256) type value there are another two function which functions the assert and revert methods and take only one input as parametre .
->write require method with some condition  which ensures that if value is not divisible by 2 then that number is odd and the count of oddcount will increse. if not then an error message will revert same with other two methods.
->click on compile (odd_even.sol)
->go to deploy and deploy it.

code blocks for commands

// SPDX-License-Identifier: MIT
pragma solidity ^0.8.17;

contract odd_even {
    uint public oddcount;

    function requireOddNumber(uint value) external {
        require(value % 2 != 0, "The number you inputted is EVEN");
        ++oddcount;
    }

    function assertoddNumber(uint value) external {
        assert(value % 2 != 0);
        ++oddcount;
    }

    function revertoddNumber(uint value) external {
        if (value % 2 == 0) {
            revert("The number you inputted is EVEN");
        }
        ++oddcount;
    }
}

## Help

Change the compiler solidity version if error occur , then change by going to compiler solidity menu present on left side of the compiler and change the compiler version.

## Authors

->Amrita Kumari
->https://www.linkedin.com/in/amrita-kumari-753319232/

## License

This project is licensed under the MIT License - see the licence file for details.
