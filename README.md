# simple-unit-test
UNIT TESTING is a level of software testing where individual units/ components of a software are tested.  
**Source:** https://www.youtube.com/watch?v=XsFQEUP1MxI  

**Nice Comment**  
The main reason to write tests first (TDD) is that the test becomes the first client/user of that code, or more specific; the first client of that API. If the tests are easy to understand the API is probably good. When I started out with TDD I ended up in situations where I felt like "the tests doesn't let my write the code I want to write, this is stupid!". It was only later I realised that my designs, code and APIs was s*it and I should listen to the tests telling me that. If tests are hard to write, the design is either bad or I'm writing some horrible integration code (filesystem, network, db).  

The other reason to have a test failing before writing the implementation is to ensure the test is testing what you think it is.
For example, making the code just throw an error to "make the test fail" would be missing the point. It's not the test that is failing, it's the implementation that fails the test. I would suggest having the test tell you what went wrong: i.e "Expected a total of: 808, was: 0". Now we can see that we are testing for the case we think we are. In the end it's really about building confidence in the tests.
