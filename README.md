# CFSTsteel
CFSTsteel model is an uniaxial material model which can be used to simulate the cyclic behavior of steel tube in concrete-filled steel tube beam-columns including local buckling.

uniaxialMaterial CFSTsteel $mat_Tag $E0 $fy $b2 $sigma_cm $a $sigma_rm $b3 $Lamda_t $Lamda_cp $Lamda_a $Lamda_yp $Lamda_r $c_t $c_cp $c_a $c_yp $c_r $Qinf $b $N $C $gamma

```
$mat_Tag, integer, Integer tag identifying material
$E0, float, Young's modulus
$fy, float, Initial yield stress
$b2, float, Compressive strain-hardening ratio
$sigma_cm, float, Compressive capping stress (Negative value; For elastic-plastic buckling its absolute value should exceed $fy)
$a, float, Softening rate of the post-buckling strength
$sigma_rm, float, Residual stress at local buckling wave length stabilization (Negative value)
$b3, float, Ratio between post-buckling and tensile reloading strength and stiffness
$Lamda_t, float, Reference cumulative strain capacity for tensile strength (The default value is 11.0)
$Lamda_cp, float, Reference cumulative strain capacity for capping strength
$Lamda_a, float, Reference cumulative strain capacity for post-buckling behavior (The default value is 4.0)
$Lamda_yp, float, Reference cumulative strain capacity for strain hardening behavior
$Lamda_r, float, Reference cumulative strain capacity for residual strength
$c_t, float, Rate of tensile strength deterioration (The default value is 1.0)
$c_cp , float, Rate of capping strength deterioration (The default value is 1.0)
$c_a, float, Rate of post-capping strength and stiffness deterioration (The default value is 1.0)
$c_yp, float, Rate of strength hardening strength and stiffness deterioration (The default value is 1.0)
$c_r, float, Rate of residual strength deterioration (The default value is 1.0)
$Qinf, float, Isotropic hardening parameter
$b, float, Saturation rate of isotropic hardening
$N, integer, Number of backstresses
$C, float, Kinematic hardening parameter associated with backstress
$gamma, float, Saturation rate of kinematic hardening associated with backstress
```

Please use Reference [1] when citing the CFSTsteel uniaxial material model.
[1] Wang S, Wang W, Lignos D G. Uniaxial material model with softening for simulating the cyclic behavior of steel tubes in concrete‐filled steel tube beam‐columns[J]. Earthquake Engineering & Structural Dynamics, 2024, 53(13): 4032-4053.

For code inquires or bug reporting, please contact: Shiye Wang, National University of Singapore, e-mail: shiye@nus.edu.sg
