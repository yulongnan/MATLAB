# MATLAB
filename= 'C:\Users\Public\Documents\DX10 data\FX_MyDesign_LogisticFunc_X26\FX_MyDesign_LogisticFunc_X26.txt';
fileID = fopen(filename);

FormatString='%f32  %f32 %f32 %f32 %f32';   %   读取数据的类型

C = textscan(fileID ,FormatString, 'delimiter', '  ',  'HeaderLines', 3);  %  'HeaderLines', 3
MyData = [C{3} C{4} C{5}]

