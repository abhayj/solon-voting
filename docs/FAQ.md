Frequently Asked Questions - Solon
==================================

Q: Where does the name come from?
---------------------------------

A: According to Wikipedia, *Solon* was the man who wrote the first democratic 
constitution in ancient Athens. http://en.wikipedia.org/wiki/Solon

To honor him, we named Solon Voting after him. And it's a simple name that
wasn't taken.

Q: What is *delegated democracy*?
---------------------------------

A: Delegated democracy is a hybrid between representative democracy and direct
democracy. Basically, the problem with representative democracy is that you
can only delegate your powers to one elected representative (or worse, one that
doesn't even get elected), who will then *represent* your powers for the next
four years and there's nothing you can do to stop him. With the arrival of the
internet, the argument goes that a more direct form of democracy is called for
where each citizen can impact legislation directly, at any time. On the other
hand direct democracy has the problem that nobody will have the time to properly
familiarize himself with and then vote on all the issues a typical Parliament 
handles, which would lead to poor policymaking. Delegated democracy is therefore
a hybrid approach: Citizens can delegate their powers to any other citizen -
much like in representative democracy - but also they can at any time change 
their delegation, or just vote directly on an issue, so that their delegation is 
not kept "hostage" for a four year election period by a corrupt politician who
didn't keep his election promises after all.

You can read more about delegated democracy at these links:

 * http://en.wikipedia.org/wiki/Delegative_democracy
 * http://liquidfeedback.org/mission/
 * http://openlife.cc/DirectDemocracy

Q: Can Solon be used for just normal, traditional elections?
------------------------------------------------------------

A: Yes. With Solon we are primarily motivated by the rise of various delegated 
democracy platforms. But it is worth pointing out Solon could also be used to 
provide a cryptographically secure voting algorithm for traditional elections 
that wish to use e-voting instead of paper ballots. (Sadly, the current vendors 
of such systems seem to be completely ignorant of existing academic research in 
this area, in fact we are not aware of any system currently existing that 
would be even close to secure or fit for purpose.) 

As a bonus, we will implement Solon in a way that it will also be possible to 
use more modern voting methods, such as various variants of preferential voting.
This requirement comes from the fact that Liquid Feedback uses one such 
method: Schulze ranking.

Q: I'm against e-voting / e-voting doesn't work / etc...?
---------------------------------------------------------

A: If you are speaking about traditional elections, then I am also against 
e-voting. This problem space can be broken into a few different things that can
go wrong, usually all of them go wrong. For one thing, the systems sold by
e-voting vendors typically lack any security at all, or even when the vendors 
try, they are still not aware of cryptographic algorithms actually created for 
this purpose but offer some terribly naive, unfit-for-purpose solutions.

The other problem is simply that paper ballot elections work well, and trying to
replace them with a complex and expensive computer system is just not very smart
(even in the case that such a system would actually implement some secure voting
protocol, which to date has not even happened.)

Solon was not created to be used in traditional elections. (But it could be used
also for such e-voting systems if you are in that business.) The motivation
behind Solon is to enable secure voting for the burgeoning delegated democracy
movement. Here the arguments for and against e-voting have a slightly different
balance.

Delegated democracy is only practical using computers and the internet - an
active participant might want to vote and propose amendments every day. If you 
believe that delegated democracy is preferable over traditional representative 
democracy, then you are already using computers and hence e-voting. In that
case the only question is, how can we make it as secure and trusted as possible.


Q: Can I use Solon in production?
---------------------------------

A: **Definitively not.** The current code is just a mockup demonstrating code 
flow and a simple user interface. There is no cryptography at all yet, and it 
won't be complete for months (or maybe years?) to come. This is an open source
project in development. Contributors are welcome, users not yet.

Q: How can I help / contribute?
-------------------------------

See the [README.md] and [TODO.md] for how to get in touch with us and what you
can help with.

[README.md]: https://raw.github.com/henrikingo/solon-voting/master/README.md
[TODO.md]: https://raw.github.com/henrikingo/solon-voting/master/TODO.md

Q: How is Solon Voting licensed?
--------------------------------

A: All of Solon is open source and licensed as GPLv3.

As an exception, the patches against Liquid Feedback which are kept under
`liquid_feedback_patch/` are licensed with the same license as Liquid Feedback 
itself, the MIT license.

