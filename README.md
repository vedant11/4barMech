# 4barMech

Authored: vedant11, MATLAB R2021a

Plots position state for the 4-bar mechanism against input angle (crank angle)

<u>Note:</u> Can be extended to other 4-bar inversions but hasn't been tested yet

`input`: 4 link lengths, 2 params for P point

---

### Crank-Rocker Mechanism

![image](https://user-images.githubusercontent.com/47473330/139678075-80994375-0814-4cba-87ef-3d3ec7681836.png)

Generating data:

1. Run `FourBar_angles.mlx` with link length inputs. The input angle steps are 5 degress by default.
2. Generated data is stored in `FourBarAngles.csv`.
3. Execute `couplePoint.mlx` with 2 params for P. This generates the path covered by P for a complete rotation of the crank.
4. You may run the following command to get a visualization:
    > stackedplot(T); % T stands for Table here, stored in the workspace

---

### SliderPin

`sliderPinCrankRocker.mlx`

![image](https://user-images.githubusercontent.com/47473330/139686869-01c50e2c-410e-487d-ba29-ffd53fecb625.png)
