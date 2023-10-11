# foward_chaining_AI_prolog


%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
% Problem: Implement advisor, a forward-chaining expert system 
% that advises UNCG undergraduate students on required and 
% elective CSC courses to take. First the advisor has a dialog
% with the student about what CSC courses he has passed and 
% what topics he likes. Then the advisor uses forward chaining 
% rules to recommend courses to the student. The advisor should 
% only recommend required courses if the student has passed 
% their prerequisites and only recommend electives if they
% are on topics interesting to the student. (If you don't know
% about UNCG courses, go to the department's computer science
% web pages to get the information you need.)

% Here are some sample interactions. Note that the FC rule
% interpreter wrote "Derived: ", and "No more facts". You
% can ask the user for information using any questions that
% you wish.

% ?- advisor.
% What required courses have you passed?
% CSC130?: y
% CSC230?: y
% CSC330?: n
% ... etc.
% Derived: take_csc330
% Derived: take_csc350
% No more facts.

% ?- advisor.
% What required courses have you passed?
% ...
% CSC350?: y
% CSC330?: y
% CSC429?: n
% ...
% What topics do you like?:
% HCI?: n
% AI?: y
% ....
% Derived: take_CSC429
% No more facts


% Directives (must be at the top of your SWI Prolog program.
% Syntax may differ in other Prolog interpreters. This is
% needed so the program can assert the fact predicate.
