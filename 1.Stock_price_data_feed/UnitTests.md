### Unit Tests:

Unit tests are useful in software development for a bunch of reasons:
- It helps increase developer's confidence in the code they write.
- It helps us to design better robust / maintainable / reusable code.
- It helps us document how our code works for other developers to use.
- It helps us catch errors in code modifications early on.

- Unit tests have nothing to do with having a running client application. - They run independently from the main application and exist for the reasons stated above. 
- The test cases we feed into the methods we test for
represent the use cases we anticipate for those methods.
  
- In unit testing, we always follow the pattern, Build-Act-Assert:
  - Build: We first build a simulated test scenario e.g. instantiating the
dummy data we will pass in the methods we’ll test, importing the class
whose methods we want to test, etc.
  - Act: We then make some operations and call the method we want to test
for
  - Assert: We check if the output of the method we’re testing matches the
expectation we have (e.g. dummy / static data of the outcome)

- Unit tests mostly use static / dummy data to represent the test cases we pass
into methods and the expected outcome of these methods when such test
cases are given. This is fine because we want our methods and tests to be
deterministic and not randomly failing / behaving in a different way we don’t
expect.
- An assertion would look something like the following bullet points below:
        
        self.assertEqual(getDataPoint(quote),dataPoint)
        self.assertEqual(1,1)

  - For more examples on assertions in python unit testing check this 'https://docs.python.org/2.7/library/unittest.html#assert-methods' or other online resource about Python unit testing.
  - As a rule of thumb, aim to use only one assertion. Use the strongest
assertion you can think of. 