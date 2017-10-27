X = 1:10;
load('results_gaussianSVR_SCUT_vgg7_50')
Ann_MAE = MAE;
Ann_PC = PC;
Ann_RMSE = RMSE;
Ann_E = E;
load('results_gaussianSVR_SCUT_vgg7_50')
Ann_MAE_W = MAE;
Ann_PC_W = PC;
Ann_RMSE_W = RMSE;
Ann_E_W = E;
load('results_gaussianSVR_SCUT_vgg7_50')
MAE = MAE;
PC = PC;
RMSE = RMSE;
E = E;
load('results_gaussianSVR_SCUT_vgg7_50')
MAE_W = MAE;
PC_W = PC;
RMSE_W = RMSE;
E_W = E;
subplot（2,2,1);
plot(X,Ann_MAE,'b--',X,Ann_MAE_W,'r--',X,MAE,'y-',X,MAE_W,'k-');
title('MAE');

subplot（2,2,2);
plot(X,Ann_PC,'b--',X,Ann_PC_W,'r--',X,PC,'y-',X,PC_W,'k-');
title('PC');

subplot（2,2,3);
plot(X,Ann_RMSE,'b--',X,Ann_RMSE_W,'r--',X,RMSE,'y-',X,RMSE_W,'k-');
title('RMSE');

subplot（2,2,4);
plot(X,Ann_E,'b--',X,Ann_E_W,'r--',X,E,'y-',X,E_W,'k-');
title('E');