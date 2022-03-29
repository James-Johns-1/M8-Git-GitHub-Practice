# James Johns

% This code uses the cross-product method to determine the 3-dimensional 
% moment about point O caused by the force F in the diagram

syms i j k % Creates symbolic variables
PosVecOB = 1 * i + 4 * j + 2 * k; % The position Vector of OB
PosVecB = 1 * i + 4 * j + 2 *k; % The Position Vector of B
PosVecC = 5 * i; % The Position Vector of C

PosVecBC = PosVecC - PosVecB; % Code to determine the position vector BC from the ones above

UnitVecBC = PosVecBC / sqrt(4^2 + (-4)^2 + (-2)^2); % Code to calculate the
% unit vector of BC

ForceVecF = (120/3) * (2 * i - 2 * k - k); % Code to calculate the force vector of F

% Mo = PosVecO * ForceVecF = PosVecOB * ForceVecF
% ^^ the cross product method ^^
Mo = 40 * ((-4+4) * i - (-1 -4) * j + (-2-8) * k);
Mx = 40 * ((-4+4) * i) % Component form of x
My = 40 * ((-1 -4) * j) % Component form of y
Mz = 40 * ((-2-8) * k) % Component form of z
