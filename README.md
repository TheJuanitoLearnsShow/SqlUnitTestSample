# SqlUnitTestSample
Sample project showing how to use automated testing for SQL Projects

It uses XUnit dynamic testing for finding SPs that define the testing. Each SP follows a results convention for pass/fail.

The xunit proj reads the name of its own proj and looks for the dacpac with the same name in the parent directories. It then publishes the dacpac to local db. It does the same wiht the ".dbtests" companion sql proj (whihc actually has the the test sps).