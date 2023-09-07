# Smart-Contract-Voting-Project
This Smart Contract Voting Project utilizes the Solidity language. It essentially comprises an Election Commissioner who oversees the conduct of free and fair elections, Candidates who participate in the election, and eligible Voters.

# Project Explanation:

I have taken a voter struct to store voter details and also a candidate struct to store candidate details.

The contract is designed  to be deployed by the Election Commissioner, who is responsible for setting the start and end times for the election process. He/She also possess the authority to halt the election in emergency situations.

This contract is designed to accommodate only two candidates participating in the election.

The candidateRegister function is responsible for candidate registration. The conditions for registration include the candidate not being an election commissioner, the candidate's age being greater than or equal to 18, and preventing duplicate registrations.

The candidateVerification function returns false if a registered candidate attempts to register again.

The candidateList function provides candidate details in array format.

The voterRegister function handles voter registration. Eligibility criteria include the voter's age being greater than or equal to 18 and preventing duplicate registrations.

The voterVerification function returns false if a registered voter attempts to register again.

The voterList function presents voter details in array format.

The vote function validates several criteria for voting, including ensuring that voters do not vote more than once, that only registered individuals are eligible to vote, and that voters can only cast their ballots for registered candidates.

The voteTime function manages the scheduling of election timings.

The votingStatus function provides details regarding the election process, such as whether voting has begun, ended, or is in progress.

The result function determines the election winner.

The emergency function is responsible for halting the election process in emergency situations.
