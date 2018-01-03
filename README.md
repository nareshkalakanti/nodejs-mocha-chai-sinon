
Testing JavaScript for Node.js and Mocha , Chai & Sinon


Mocha :For writing unit test
Chai for asserts
* Sinon for mocking
* Istanbul for code coverage
Note : Node changes fast and how to fix and monitor when the release cycle is 3 months

Unit vs Integration vs functional

* Unit Test
    * Find the smallest available piece
    * Test just that
    * Mock everything else
* Integration
    * Lets tie some things together
    * Test their interactions
    * Mock the outside resources
* Function Tests
    * All together
    * Start on the outside , end on the outside
    * Black box testing : I don’t have idea whats going on inside the application
    * Make sure everything fits together
* Dealing with Node Versions ?
    * Since they have a very aggressive release cycle
    * Nvm to the Rescue
    * Install node version manager
        * Terminal > which node > nvm install 7.9 [latest version node ] > nvm use — lts
    * Switch between node version


Testing with Mocha
* Mocha as a test runner
* Mechanism by which tests are executed
* Describes and its …
* Lifecycle Hooks
* Managing what tests execute

Note : Clean up asserts using CHAI


    BDD Style Assertions

* Assert is clunky
* Chai for better assertions
    * Two Options
        * expect
        * should
* Verifying objects
* BDD is Descriptive


* Example

        describe('isAuthorized', function () {
        it('Should return false if not authorized', function (done) {
        function (done) {

  expect(something).to.be
                                    .equal
                                    .have
                                    .true

Spys , Stubs, and Mocks
    * Testing is not always straight forward
    * Mocking objects is required to unit test
    * Sinon to rescue
Spy gives us a fake function to test some thing
    Ex
        var func = sinon.spy( )
We can use this to track execution

Stubs for replacing objects

Mocks
*     Mocks are fake methods (likes spies) with pre-programmed behaviour (like stubs) as well as pre-programmed expectations.
* Mocks for easier expectations



Notes :
* Testing is not always straightforward
* Databases and HTTP calls add Complications




