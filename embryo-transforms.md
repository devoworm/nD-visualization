Done with *C. elegans* embryo point cloud.

x = A(:,1);  
y = A(:,2);  
v = 2*(x.*y);  
scatter3(v,x,y,"red","fill","o");  
// saddle-shaped space.  


scatter3(u,x,y,"red","fill","o");  
// u-shaped bend around x=0. Concave curvature about z-axis.  

u = sqrt(x^2+y^2+z^2);  
scatter3(u,x,y,"red","fill","o");  
// u-shaped bend around x=0. Convex curvature about z-axis.  
