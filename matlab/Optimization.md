
MATLAB 中包括 Optimization 和 Global Optimization两个优化工具箱,其中 Optimization 的描述为:
<blockquote>
Optimization Toolbox™ provides functions for finding parameters that minimize or maximize objectives while satisfying constraints. The toolbox includes solvers for linear programming, mixed-integer linear programming, quadratic programming, nonlinear optimization, and nonlinear least squares.  You can use these solvers to find optimal solutions to continuous and discrete problems, perform tradeoff analyses, and incorporate optimization methods into algorithms and applications.
  
优化工具箱Optimization Toolbox™提供了一些函数用于搜索使满足约束条件的对象最大化或最小化的参数。工具箱中包括一些求解器，用于线性规划，混合-整数线性规划，二次规划，非线性优化，和非线性最小二乘法。你可以使用这些求解器来搜索连续和离散问题的最优解，进行权衡分析，并且在算法和应用中嵌入优化方法。

<H3>Key Features</H3>
<ul>
<li> Nonlinear and multiobjective optimization（非线性和多对象优化）</li>
<li>- Solvers for nonlinear least squares, data fitting, and nonlinear equations（非线性最小二乘法，数据拟合和非线性方程组的求解器）</li>
<li>- Quadratic and linear programming（二次和线性规划）</li>
<li>- Mixed-integer linear programming（混合-整数线性规划）</li>
<li>- Optimization app for defining and solving optimization problems and monitoring solution progress（用于定义和解决优化问题，以及检测求解过程的优化工具app）</li>
<li>- Acceleration of constrained nonlinear solvers with Parallel Computing Toolbox™（使用并行计算工具箱加速受约束非线性求解器）</li>
</ul>
</blockquote>
而 Global Optimization工具箱的描述为：
<blockquote>
  Solve multiple maxima, multiple minima, and nonsmooth optimization problems
  求解多元极大值，多元极小值，和非平滑优化问题
  Global Optimization Toolbox provides methods that search for global solutions to problems that contain multiple maxima or minima. It includes global search, multistart, pattern search, genetic algorithm, and simulated annealing solvers. You can use these solvers to solve optimization problems where the objective or constraint function is continuous, discontinuous, stochastic, does not possess derivatives, or includes simulations or black-box functions with undefined values for some parameter settings.
  全局优化工具箱Global Optimization Toolbox提供了一些用于搜索包含多元极大值或多元极小值全局解的方法。包括全局搜索，多起点方法，模式搜索，遗传算法，和模拟退火求解器。你可以使用这些求解器去解决优化问题，目标函数或约束条件可以是连续，不连续，随机化，不可导，或包括仿真或在某些参数设置中存在未定义值的黑箱函数。
  Genetic algorithm and pattern search solvers support algorithmic customization. You can create a custom genetic algorithm variant by modifying initial population and fitness scaling options or by defining parent selection, crossover, and mutation functions. You can customize pattern search by defining polling, searching, and other functions.
  遗传算法和模式搜索求解器支持个性化算法。你可以通过修正初始群体和拟合尺度选项，或者定义父代选择，交叉重组，和突变函数来创建一个个性化的遗传算法变量。你可以通过定义聚合，搜索和其他函数的方式来个性化的进行模式搜索。
<H3>Key Features</H3>
 <ul>
<li>Interactive tools for defining and solving optimization problems and monitoring solution progress</li>
<li>Global search and multistart solvers for finding single or multiple global optima</li>
<li>Genetic algorithm solver that supports linear, nonlinear, and bound constraints</li>
<li>Multiobjective genetic algorithm with Pareto-front identification, including linear and bound constraints</li>
<li>Pattern search solver that supports linear, nonlinear, and bound constraints</li>
<li>Simulated annealing tools that implement a random search method, with options for defining annealing process, temperature schedule, and acceptance criteria</li>
<li>Parallel computing support in multistart, genetic algorithm, and pattern search solver </li>
<li>Custom data type support in genetic algorithm, multiobjective genetic algorithm, and simulated annealing solvers</li>
</ul>
</blockquote>

总的来说，优化工具箱提供的方法倾向于获得局部最优解，而全局优化工具箱则更倾向于获得全局的最优解。


