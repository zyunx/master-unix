=====================
Make a Disk from Tape
=====================

Integrity Checks
Integrity checks may be applied for each byte or on the groups of bytes forming a link-level transmisison frame.

Character Parity
Character or byte parity is an error detection technique that is typically used with asynchronous links. It is used to verify the integrity of each individual received byte. When used, each character (byte) is protected at the sender by one additional single parity bit, which is the logical exclusive or of all the bits in each byte.

Longitudinal Parity Checksum
A frame integrity check protects all the bytes in a frame. It seeks to verify if the whole farme is correct (i.e. can not identify in which byte an error occurs, but instead just tells if there have been any detected errors within the entire frame).

The simplest form of frame integrity check is the longitudinal paritry checksum. This consists of an additional byte added at the end of each transmisison frame by the sender. The receiver performs the same opeartion as the sender and compares the calculated value with the received checksum. If both match the frame, then the frame is judged to be valid. If not, it is invalid (and will usually be discarded by the receiver).

more to see: https://erg.abdn.ac.uk/users/gorry/eg3576/checksums.html
