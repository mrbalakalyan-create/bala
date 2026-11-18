import React, { useState } from 'react';

function Countersss() {

    //usestate syntax
    const [count, setCount] = useState(0);

    const handleIncrease = () => {
        setCount(count + 1);
    };

    const handleDecrease = () => {
        setCount(count - 1);
    };

    return (
        <div>
            <p style={{ color: count > 0 ? "green" : count < 0 ? "red" : "yellow" }}>{count}</p>

            <button onClick={handleIncrease}>+</button>
            <button onClick={handleDecrease}>-</button>
        </div>
    );
}

export default Countersss;
