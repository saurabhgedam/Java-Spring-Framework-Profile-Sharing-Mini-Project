# Java-Spring-Framework-Profile-Sharing-Mini-Project

The project implements the athurization aspect and the retry aspect for the following set of profile sharing rules:
- Once can share his profile with anybody.
- One can only read profiles that are shared with him, or his own profile. In any other case, an AccessDeniedExeption is thrown.
- If Alice shares her profile with Bob, Bob can further share Alice’s profile with Carl. If Alice attempts to share Bob’s profile with Carl while Bob’s profile is not shared with Alice in the first place, Alice gets an AccessDeniedExeption.
- One can only unshare his own profile. When unsharing a profile with Bob that the profile is not shared by any means with Bob in the first place, the operation throws an AccessDeniedExeption. 
- Both sharing and unsharing of Alice’s profile with Alice have no effect; i.e. Alice always has access to her own profile, and can share and unshare with herself without encountering any exception, even these operations do not take any effect.
