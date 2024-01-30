The optimized airfoils, initial airfoils, the parameters, 
and performance data of the optimized designs can all be 
found as npy arrays in the train, test, and val folders.
Alternativley, you can choose to load it all at once  
from the train_test_val_opt.pkl and 
train_test_val_opt_params.pkl files;
i.e 
train, test, val = pd.read_pickle(fname)

Parameters in order:

mach : mach number
reynolds : reynolds number 
cl_target : target coeff. of lift
area_target: target minimum allowable area 
alpha : optimized angle of attack
area_initial : initial area 
cd_val : optimized coeff of drag (In drag counts: 1 drag count = 0.0001)
cl_val : optimized coeff of lift
cl_con : coeff of lift constraint satisfaction
area_con : area constrain satisfaction