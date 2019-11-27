# pytest-unordered

Test equality of unordered collections in pytest.

## Installation

    pip install pytest-unordered
    

## Usage

    from pytest_unordered import unordered
    
    def test_unordered():
        assert [3, 2, {1: ['a', 'b']}] == unordered([{1: ['a', 'b']}, 2, 3])
