Done with *C. elegans* embryo point cloud as the source of data. Coding done in SciLab 6.0:  

x = A(:,1);  
y = A(:,2);  
v = 2*(x.*y);  
scatter3(v,x,y,"red","fill","o");  
// saddle space.  

Saddle space might require a PCA transformation:  
a = [data];
[lambda,facpr,comprinc] = pca(a);
x = comprinc(:,1);  
y = comprinc(:,2);  
v = 2*(x.*y);  
scatter3(v,x,y,... 
"markerEdgeColor", "black",...  
"markerFaceColor", [.8 .2 .2]);  

scatter3(u,x,y,"red","fill","o");  
// u-shaped bend around x=0. Concave arrow, u-shaped bend.  

u = sqrt(x^2+y^2+z^2);  
scatter3(u,x,y,"red","fill","o");  
// u-shaped bend around x=0. Concave arrow, u-shaped bend.  

x = A(:,1);
y = A(:,2);
z = A(:,3);
uu = %pi*(sqrt(x^2+y^2));
// v-space, z-oriented.

x = A(:,1);
y = A(:,2);
uuu = %pi*(x^2.*y^2);
v = 2*(x.*y);
z = A(:,3);
// circular band, z-oriented
